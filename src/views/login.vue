<template>
    <div class='login'>
        <div class="logo">
            <div class="logo-img"></div>
        </div>
        <div class="login-box">
            <div class="login-btn">手机号登录</div>
            <div class="three-login-box">
                <a href="#" class="three-login-item"></a>
                <a href="#" class="three-login-item"></a>
                <a href="#" class="three-login-item"></a>
                <a href="#" class="three-login-item"></a>
            </div>
            <div class="login-agreement">
                <input id="login" type="checkbox" name="agree"><span class="agree">同意</span>
                <p>《用户协议》&nbsp;《隐私政策》&nbsp;《儿童隐私政策》</p>
            </div>
        </div>
    </div>
</template>
<script>
    export default {
        name: 'login',
        data() {
            return {}
        },
        methods: {}
    }
</script>
<style lang='scss' scoped>
@import "@/assets/css/common.scss";
@import "@/assets/css/reset.scss";
     ::v-deep.login{
        position: relative;
        height: 100%;
        width: 100%;
        background-color: $baseColor;
        .logo{
            position: absolute;
            left: 50%;
            top: 180px;
            transform: translateX(-50%) translateY(-50%);
            width: 100px;
            height: 100px;
            border-radius: 50%;
            background: red url("../assets/icons/logo.png") no-repeat center;
            background-size: 70%;
        }
        .login-box{
            position: absolute;
            bottom: 20px;
            left: 50%;
            width: 80%;
            transform: translateX(-50%);
            .login-btn{
                width: 100%;
                height: 40px;
                margin-bottom: 20px;
                text-align: center;
                line-height: 40px;
                font-size: 16px;
                color:$baseColor;
                border-radius: 20px;
                letter-spacing: 2px;
                background-color: white;
            }
            .three-login-box{
                display: flex;
                justify-content: space-around;
                width: 100%;
                .three-login-item{
                    display: block;
                    width: 30px;
                    height: 30px;
                    border: 1px solid white;
                    border-radius: 50%;
                    box-sizing: border-box;
                    background-size: 22px;
                    background-repeat: no-repeat;
                    background-position: center;
                    &:nth-child(1){
                        background-image: url("../assets/icons/weixin_logo.png");
                        background-position: 50% 60%;
                    }
                    &:nth-child(2){
                        background-image: url("../assets/icons/qq_logo.png");
                    }
                    &:nth-child(3){
                        background-image: url("../assets/icons/weibo_logo.png");
                    }
                    &:nth-child(4){
                        background-image: url("../assets/icons/wangyi_logo.png");
                    }
                }
            }
            .login-agreement{
                display: flex;
                justify-content: center;
                width: 100%;
                margin-top: 20px;
                #login{
                    width: 15px;
                    height: 15px;
                    border-radius: 2px!important;
                    border: 1px solid #999;
                    margin-right: 5px;
                    background-color: unset!important;
                }
                span{
                    color: #999;
                    line-height: 17px;
                }
                p{
                    color: white;
                    line-height: 17px;
                    font-weight: lighter;
                }
            }
        }
    }
</style>