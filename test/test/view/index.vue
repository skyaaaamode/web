<template>
    <div>
        <h-form :model="setting" :label-width="100">
            <h-form-item label="自动切换">
                <h-switch v-model="setting.autoplay">
                    <span slot="open">开</span>
                    <span slot="close">关</span>
                </h-switch>
            </h-form-item>
            <h-form-item label="自动切换速度">
                <h-slider v-model="setting.autoplaySpeed" :min="300" :max="10000" :step="100"></h-slider>
            </h-form-item>
            <h-form-item label="指示器位置">
                <h-radio-group v-model="setting.dots" type="button">
                    <h-radio label="inside">内部</h-radio>
                    <h-radio label="outside">外部</h-radio>
                    <h-radio label="none">不显示</h-radio>
                </h-radio-group>
            </h-form-item>
            <h-form-item label="切换箭头">
                <h-radio-group v-model="setting.arrow" type="button">
                    <h-radio label="hover">悬停时显示</h-radio>
                    <h-radio label="always">一直显示</h-radio>
                    <h-radio label="never">不显示</h-radio>
                </h-radio-group>
            </h-form-item>
            <h-form-item label="指示器触发方式">
                <h-radio-group v-model="setting.trigger" type="button">
                    <h-radio label="click">点击</h-radio>
                    <h-radio label="hover">悬停</h-radio>
                </h-radio-group>
            </h-form-item>
        </h-form>
        <h-carousel
                v-model="value3"
                :autoplay="setting.autoplay"
                :autoplay-speed="setting.autoplaySpeed"
                :dots="setting.dots"
                :trigger="setting.trigger"
                :arrow="setting.arrow">
            <h-carouselitem>
                <div class="demo-carousel">1</div>
            </h-carouselitem>
            <h-carouselitem>
                <div class="demo-carousel">2</div>
            </h-carouselitem>
            <h-carouselitem>
                <div class="demo-carousel">3</div>
            </h-carouselitem>
            <h-carouselitem>
                <div class="demo-carousel">4</div>
            </h-carouselitem>
        </h-carousel>
    </div>
</template>
<style>
    .demo-carousel {
        height: 200px;
        line-height: 200px;
        text-align: center;
        color: #fff;
        font-size: 20px;
        background: #506b9e;
    }
</style>
<script>
    export default {
        data () {
            return {
                value3: 0,
                setting: {
                    autoplay: false,
                    autoplaySpeed: 2000,
                    dots: 'inside',
                    trigger: 'click',
                    arrow: 'hover'
                }
            }
        },
    }
</script>