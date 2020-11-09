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
            <!--模块展示区域-->
            <div id="mid-show-banner">
                <!--左边的背景地图-->
                <div class="back-image"></div>
                <!--注册框-->
                <div id="register-box" class="input-area">
                    <div class="switch-qrcode" >
                        <div id="switch-qr" class="switch-signal"></div>
                    </div>
                    <div id="step-1" class="register-content-box">
                        <div class="switch-login">
                            <button class="box-button  btn-without-border">登录</button>
                            <button class="box-button btn-without-border button-active">注册</button>
                        </div>
                        <div id="tel" class="segmentation-icon">
                            <input autocomplete="off" placeholder="手机号" type="text" rows="2" validateevent="true"
                                   class="login-input-text">
                        </div>
                        <div class="verification-code segmentation-icon space-between">
                            <input autocomplete="off" placeholder="验证码" type="text" rows="2" validateevent="true"
                                   class="login-input-text verify-text">
                            <div id="verfify-code-register"></div>
                        </div>
                        <div class="verification-code segmentation-icon space-between">
                            <input autocomplete="off" placeholder="手机验证码" type="text" rows="2" validateevent="true"
                                   class="login-input-text verify-text">
                            <div class="verfify-get">
                                <button class="get-verify-btn">获取验证码</button>
                            </div>
                        </div>
                        <div id="password-register" class="segmentation-icon">
                            <input autocomplete="off" placeholder="密码" type="password" rows="2" maxlength="20"
                                   minlength="8" validateevent="true" class="login-input-text">
                        </div>
                        <div id="repassword" class="segmentation-icon">
                            <input autocomplete="off" placeholder="确认密码" type="password" rows="2" maxlength="20"
                                   minlength="8" validateevent="true" class="login-input-text">
                        </div>
                        <div class="check-agreement">
                            <div class="checkBox"><input type="checkbox"></div>
                            我已经阅读并同意
                            <a>《恒生服务协议》</a>
                        </div>
                        <div>
                            <button id="next-btn" disabled="disabled" class="btn-register-box">下一步</button>
                        </div>

                    </div>
                    <div id="step-2" class="register-content-box">
                        <div class="switch-login">
                            <button class="box-button  btn-without-border">登录</button>
                            <button class="box-button btn-without-border button-active">注册</button>
                        </div>
                        <div id="name" class="segmentation-icon">
                            <input autocomplete="off" placeholder="姓名" type="text" rows="2" validateevent="true"
                                   class="login-input-text">
                        </div>
                        <div id="mail" class="segmentation-icon">
                            <input autocomplete="off" placeholder="邮箱" type="text" rows="2" validateevent="true"
                                   class="login-input-text">
                        </div>
                        <div class="verification-code segmentation-icon space-between">
                            <input autocomplete="off" placeholder="验证码" type="text" rows="2" validateevent="true"
                                   class="login-input-text verify-text">
                            <div id="tel-verify-code"></div>
                        </div>
                        <div class="verification-code segmentation-icon space-between">
                            <input autocomplete="off" placeholder="手机验证码" type="text" rows="2" validateevent="true"
                                   class="login-input-text verify-text">
                            <div class="verfify-get">
                                <button class="get-verify-btn">获取验证码</button>
                            </div>
                        </div>
                        <div id="company-name" class="segmentation-icon">
                            <input autocomplete="off" placeholder="公司名称" type="text" rows="2" validateevent="true"
                                   class="login-input-text">
                        </div>
                        <div id="team-name" class="segmentation-icon">
                            <input autocomplete="off" placeholder="团队名称" type="text" rows="2" validateevent="true"
                                   class="login-input-text">
                        </div>
                        <div class="check-agreement">
                            <div class="checkBox"><input type="checkbox"></div>
                            <div>信息确认无误，提交后无法修改</div>
                        </div>
                        <div>
                            <button id="register-btn" class="btn-register-box">注册</button>
                        </div>

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

                                    <li class="hs_link_sigal_loc"><a href="http://service.hundsun.com/"
                                                                     target="_blank">恒生客服</a>
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

<script>
    export default {
        data() {
            return {
                pageType: "login",
                loginType: "text",
            }
        },
        methods: {
            switchLoginType: function () {
                if ("text" === this.loginType) {
                    document.getElementById("origin").style.opacity = "0";
                    document.getElementById("origin").style.display = "none";
                    document.getElementById("qr-login").style.display = "block";
                    document.getElementById("qr-login").style.opacity = "1";
                    this.loginType = "qrCode";
                } else {
                    document.getElementById("qr-login").style.opacity = "0";
                    document.getElementById("qr-login").style.display = "none";
                    document.getElementById("origin").style.display = "block";
                    document.getElementById("origin").style.opacity = "1";
                    this.loginType = "text";
                }

            }

        }
    }
</script>