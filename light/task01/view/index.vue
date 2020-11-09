<template>
    <div>
        <div id="main_desk">
            <div class="wrap-top">
                <div id="topBar" class="topBar">
                    <div id="topBar_left" class="topBar_left">
                        <div class="topBar_icon">
                            <img class="topBar_signal" src="../images/logoProductName.png">
                        </div>
                        <div class="topBar_signal_02" ></div>
                        <div class="topBar_text">恒生移动开发平台</div>
                    </div>
                    <div id="topBar_right" class="topBar_right">
                        <ul>
                            <li><a href="javascript:void (0)">文档中心</a></li>
                            <li><a href="javascript:void (0)">控制台</a></li>
                            <li><button class="login" @click="toLogin($event)" data-index="APP">登录</button></li>
                            <li><button class="register">注册</button></li>
                        </ul>
                    </div>
                </div>

            </div>
            <div class="description">
                <div>
                    <h-carousel :autoplay=autoPlayContraller :autoplay-speed="10000" v-model="value4" arrow="never" @on-change="change">
                        <h-carouselitem>
                            <div class="demo-carousel">
                                <div id="app_banner">
                                    <div  class="index_info">
                                        <h1>APP</h1>
                                        <span>基于WEB开发体验的移动开发平台，帮助企业开发者更高效率、更高用户体验的构建超级APP。</span>
                                        <button class="btn-primary-1" onclick="f3()">开始使用</button>
                                    </div>
                                    <div class="bannerright">
                                        <div class="app_left"></div>
                                        <div class="app_mid mid"></div>
                                        <div class="app_right"></div>
                                    </div>
                                    <div>
                                    </div>
                                </div>
                            </div>
                        </h-carouselitem>
                        <h-carouselitem>
                            <div class="demo-carousel">
                                <div id="H5_banner">
                                    <div  class="index_info">
                                        <h1>H5</h1>
                                        <span>基于WEB开发体验的移动开发平台，帮助企业开发者更高效率、更高用户体验的构建超级APP。</span>
                                        <button class="btn-primary-1">开始使用</button>
                                    </div>
                                    <div class="bannerright">
                                        <div class="H5_left"></div>
                                        <div class="H5_mid mid"></div>
                                        <div class="H5_right"></div>
                                    </div>

                                </div>

                            </div>
                        </h-carouselitem>
                        <h-carouselitem>
                            <div class="demo-carousel">
                                <div id="mini_banner">
                                    <div  class="index_info">
                                        <h1>小程序</h1>
                                        <span>基于WEB开发体验的移动开发平台，帮助企业开发者更高效率、更高用户体验的构建超级APP。</span>
                                        <button class="btn-primary-1">开始使用</button>
                                    </div>
                                    <div class="bannerright">
                                        <div class="mini_left"></div>
                                        <div class="mini_mid mid"></div>
                                        <div class="mini_right"></div>
                                    </div>

                                </div>
                            </div>
                        </h-carouselitem>
                    </h-carousel>
                </div>
            </div>
        </div>
        <div class="index_info_mid_word">
            <div class="desc">
                <h1 align="center" style="z-index: 2">GMU恒生移动开发平台</h1>
                <span style="z-index: 2">更易用的移动终端开发服务平台，提升产品交付效率，帮助产品快速迭代</span>
                <button class="btn-primary-2" style="z-index: 2">立即注册</button>
            </div>
            <div class="backimg"><img src="../images/backgroundBlue.png" style="z-index:-1;height: 100%;width: 100%"></div>
        </div>
        <div id="index_info_down" class="index_info_down">
            <div id="hs_link" class="hs_link">
                <div id="link_left" class="link_left">
                    <div>
                        <div>
                            <ul>
                                <li class="line_signal" style="line-height: 20px">
                                    <div style="display: inline-block;width: 100%">友情链接</div>
                                    <div class="link_line_hr" style="display: inline-block"></div>
                                </li>

                                <li class="hs_link_sigal_loc"><a href="http://service.hundsun.com/" target="_blank">恒生客服</a>
                                </li>
                                <li><a href="http://www.hundsun.com/" target="_blank">恒生电子</a></li>
                                <li><a href="http://rdc.hundsun.com/portal/" target="_blank">恒生研究院</a></li>
                                <li><a href="http://www.hs.net/" target="_blank">恒生云</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div id="link_mid" class="link_mid">
                    <div class="link_ul">
                        <ul>
                            <li class="line_signal" style="line-height: 20px">
                                <div style="display: inline-block;width: 100%">支持与服务</div>
                                <div class="link_line_hr" style="display: inline-block"></div>
                            </li>
                            <li class="hs_link_sigal_loc">
                            <span><div style="margin-right: 5px"><img src="../images/signalLoc.png"></div>
                                地址：浙江省杭州市滨江区江南大道3588号</span>
                            </li>
                            <li>
                            <span><div style="margin-right: 5px"><img src="../images/signalTel.png"></div>
                                电话：0571-28828888</span>
                            </li>
                            <li>
                            <span><div style="margin-right: 5px"><img src="../images/signalMail.png"> </div>
                                邮箱：service@hundsun.com</span>
                            </li>
                            <li>
                             <span><div style="margin-right: 5px"><img src="../images/signalDoc.png"> </div>
                                文档中心</span>
                            </li>

                        </ul>
                    </div>
                </div>
                <div id="link_right" class="link_right">
                    <ul>
                        <li class="line_signal" style="line-height: 20px">
                            <div style="display: inline-block;width: 100%">钉钉服务群</div>
                            <div class="link_line_hr" style="display: inline-block"></div>
                        </li>
                        <li class="hs_link_sigal_loc">
                            <div>
                                <img class="qr_code" src="../images/qrCode.png">
                            </div>
                        </li>
                    </ul>


                </div>

            </div>

        </div>
        <div id="brand" class="brand">
            <div id="brand_word">
                <span><img src="../images/signalSmile.png" class="signalSmail">Copyright© Hundsun Technologies Inc.All Rights Reserved 浙ICP备09092082号-5</span>
            </div>
        </div>
    </div>


</template>
<style>
    .demo-carousel {
        height: 591px;
        line-height: 200px;
        text-align: center;
        color: #fff;
        font-size: 20px;
        /*background: #506b9e;*/
        position: relative;
    }
    /*.h-carousel-dots li{*/
    /*  background: #D6E9FF;*/
    /*    width: 35px;*/
    /*    height: 6px;*/
    /*}*/
    .h-carousel-dots li{
        position: relative;
        display: inline-block;
        vertical-align: top;
        text-align: center;
        padding:0 0 !important;
        cursor: pointer;
        width: 60px;
        height: 3px;
        line-height: 6px;
        background: #D6E9FF;
        margin-left: 10px;
    }

    .h-carousel-dots li button {
        border: 0;
        cursor: pointer;
        display: block;
        border-radius: 1px;
        outline: none;
        font-size: 0;
        width: 60px;
        height: 3px;
        opacity: 0;
        background-color: transparent;

    }
    .h-carousel-dots li.h-carousel-active > button {
        background-image: url("../images/signalIndes.png");
        background-repeat: no-repeat;
        background-size: 60px 3px;
        background-position:left;
        width: 60px;
        opacity: 1 !important;
        animation: define 5s;
        animation-timing-function:linear;
    }
    @keyframes define {
        0%{background-position: -60px 0px }
        100%{background-position: 0px 0px }
    }


</style>
<script>
    export default {
        data () {
            return {
                value4: 0,
                autoPlayContraller:false,
                flag: {}
            }
        },
        methods: {
            change:function (oldvalue,value) {
                console.log("测试:oldvalue:"+oldvalue+", value:"+value);
            },
            toLogin:function (ev) {
                // alert(ev.currentTarget.getAttribute("data-index"));
                window.location.href="www.baidu.com?from:"+ev.currentTarget.getAttribute("data-index");

            },
            getParam:function(){
                var url = window.document.location.href.toString(); //获取的完整url
                var u = url.split("?");
                if(typeof(u[1]) == "string"){
                    u = u[1].split("&");
                    var get = {};
                    for(var i in u){
                        var j = u[i].split("=");
                        get[j[0]] = j[1];
                    }
                    return get;
                } else {
                    return {};
                }
            }
        },
        created:function () {
            var param = this.getParam();
            this.flag=param;
            alert(this.flag.flag+":"+this.flag.hellow)
        }
    }
</script>
