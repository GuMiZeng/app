<template>
<div class="login">
        <div class="close"></div>
        <div class="title">
            <span>登录</span>
        </div>
        <div class="logo">
            <img src="../src/assets/logo2_03.png" alt="logo">
        </div>
        <div class="form">
            <div class="phone">
                <img class="img_icon" src="../src/assets/tb1_03.png">
                <input type="text" id="phone" placeholder="请输入手机号">
            </div>
            <div class="password">
                <img class="img_icon" src="../src/assets/tb1_11.png">
                <input type="text" id="password" placeholder="请输入密码">
                <img class="eye" :src="eye_close">
            </div>
            <div class="remember">
                <img class="checkbox" :src="check"><span>记住密码</span>
            </div>
            <div class="login_btn"><span>登录</span></div>
            <div class="handle">
                <a href="#">忘记密码？</a>
                <a href="#">注册</a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      check: require('../src/assets/k_03.png'),
      eye_close: require('../src/assets/y2_03.png')
    }
  }
}
</script>

<style>
.login{
    /* width: 80vw; */
    height: 87.5vh;
    margin: 0 auto;
    padding: 5vh 20px;
    color: #fff;
    background: url(../src/assets/bg.png) no-repeat;
    background-size: cover;
}
.close{
    width: 18px;
    height: 18px;
    float: left;
    margin: 0 0 0 10px;
    background-image: url(../src/assets/x2_03.png);
    background-size: contain;
}
.title{
    width: 40px;
    margin: 0 auto;
    font-size: 20px;
}
.logo{
    width: 72px;
    margin: 80px auto;
}
.form{
    width: 80%;
    margin: 0 auto;
}
.phone, .password, .login_btn{
    width: 100%;
    height: 32px;
    line-height: 32px;
    padding: 5px 0;
    border: 1px solid #fff;
    border-radius: 20px;
}
.password{
    margin: 30px 0 10px 0;
}
.img_icon{
    float: left;
    width: 25px;
    height: 30px;
    margin: 0 15px;
}
.eye{
    float: right;
    margin: -20px 15px;
    width: 20px;
    height: 10px;
}
.form input{
    border: none;
    background-color: transparent;
    height: 30px;
    outline: none;
    color: #fff;
    font-size: 16px;
}
input::-webkit-input-placeholder{
    /* WebKit browsers */
    color: #fff
}
.remember{
  height: 20px;
  line-height: 20px;
}
.remember .checkbox{
  float: left;
  margin: 0 5px 0 0;
  width: 18px;
  height: 18px;
}
.login_btn{
    margin: 40px 0 10px 0;
    background-color: rgba(255, 255, 255, .3);
    border: none;
    font-size: 20px;
    text-align: center;
    letter-spacing: 4px
}
.handle{
    display: flex;
    justify-content: space-between;
}
.handle a{
    color: #fff;
    font-size: 14px;
    text-decoration: none;
}
.handle a:hover{
    text-decoration: underline;
}
</style>
