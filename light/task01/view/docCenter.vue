<template>
    <div>
        <div class="wrap-top">
            <div id="topBar" class="topBar">
                <div id="topBar_left" class="topBar_left">
                    <div class="topBar_icon">
                        <img class="topBar_signal" src="../images/logoProductName.png">
                    </div>
                    <div class="topBar_signal_02"></div>
                    <div class="topBar_text">恒生移动开发平台</div>
                </div>
            </div>

        </div>
        <div class="curve">
            <!--        搜索区域-->
            <div id="search-area">
                <div id="search-text"></div>
            </div>
<!--            模块展示区域-->
            <div id="show-banner">
                <div id="h5" class="banner">
                    <div  id="h5-icon" class="banner-icon"></div>
                    <div class="headline">H5云组件</div>
                    <div class="text">基于vue的移动HTML5应用开发、发布及安全互联网接入</div>
                    <div class="button-area">
                        <button class="show-banner-button">公众号</button>
                        <button class="show-banner-button">vue</button>
                    </div>
                </div>
                <div id="app" class="banner mid-banner">
                    <div  id="app-icon" class="banner-icon"></div>
                    <div class="headline">LightAPP</div>
                    <div class="text">基于H5的开发体验，组件化，配置化开发，运维APP</div>
                    <div class="button-area">
                        <button class="show-banner-button">APP</button>
                        <button class="show-banner-button">H5</button>
                    </div>
                </div>
                <div id="mini" class="banner">
                    <div  id="mini-icon" class="banner-icon"></div>
                    <div class="headline">小程序</div>
                    <div class="text">微信语法风格的小程序开发，可同时运行在微信和Light APP环境</div>
                    <div class="button-area">
                        <button class="show-banner-button">微信</button>
                        <button class="show-banner-button">支付宝</button>
                        <button class="show-banner-button">APP</button>
                    </div>
                </div>
                <div id="sdk" class="banner">
                    <div id="sdk-icon" class="banner-icon"></div>
                    <div class="headline">JSSDK</div>
                    <div class="text">面向APP中的跨平台开发场景，提供原生代码与前端代码间的通信，API支持</div>
                    <div class="button-area">
                        <button class="show-banner-button">APP</button>
                        <button class="show-banner-button">跨平台</button>
                    </div>
                </div>
                <div id="ui" class="banner mid-banner">
                    <div id="ui-icon" class="banner-icon"></div>
                    <div class="headline">UI</div>
                    <div class="text">提供H5，JSNative，小程序开发所需的基础UI控件，图表控件</div>
                    <div class="button-area">
                        <button class="show-banner-button">H5</button>
                        <button class="show-banner-button">JSNative</button>
                        <button class="show-banner-button">小程序</button>
                    </div>
                </div>
            </div>
            <div id="doc-separator"></div>
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
    .h-carousel-dots li {
        position: relative;
        display: inline-block;
        vertical-align: top;
        text-align: center;
        padding: 0 0 !important;
        cursor: pointer;
        width: 35px;
        height: 6px;
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
        width: 35px;
        height: 6px;
        opacity: 0;


    }

    .h-carousel-dots li.h-carousel-active > button {
        background: #387FFF;
        width: 35px;
        opacity: 1 !important;
        animation: define 10s;
    }

    @keyframes define {
        0% {
            width: 0px
        }
        100% {
            width: 35px
        }
    }

</style>
<script>
    export default {
        data() {
            return {
                value4: 0,
                autoPlayContraller: open
            }
        },
        methods: {
            change: function (oldvalue, value) {
                console.log("测试:oldvalue:" + oldvalue + ", value:" + value);
            },
            toLogin: function (ev) {
                // alert(ev.currentTarget.getAttribute("data-index"));
                window.location.href = "www.baidu.com?from:" + ev.currentTarget.getAttribute("data-index");

            },
            stopAutoplay: function () {
                this.data.autoPlayContraller = false;
            },
            openAutoplay: function (ev) {
                this.data.autoPlayContraller = true;
            }
        }
    }
</script>