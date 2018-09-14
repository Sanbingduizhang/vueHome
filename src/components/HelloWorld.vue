<template>
  <div id="box">
        <!-- 顶部
        <div class='header'>
            <div class='header-left'>
            </div>
            <div class='header-right'>
                <ul class='subZhu'>
                    <li class="li1">
                        <a id='linkZhu' href='javascript:void(0);'>注册</a>
                    </li>
                    <li>
                        <a id='linkSub' href='javascript:void(0);'>登录</a>
                    </li>
                </ul>
                <div class='head-img' title='头像名称'><img src='public/home/index/img/weixin.jpg' width='50'>
                    <div class="head-mess">
                        <ul>
                            <li><a href="#">基本资料</a></li>
                            <li><a href="#">文章信息</a></li>
                            <li><a href="#">相册信息</a></li>
                            <li><a href="#" class="loginOut">退出</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div> -->
        <!-- 中间主体部分 -->
        <div class="content">
            <!-- 注册登陆部分 -->
            <div id='coverGo'>
                    <!--<div class='login-header'><a id='link' href='javascript:void(0);'>点击，弹出登录框</a></div>-->
                    <!-- 登录功能 -->
                    <div id='login' class='login'>
                        <div id='title1' class='login-title'>登录会员
                            <span>
                                <a id='closeBtn' href='javascript:void(0);' class='close-login'>关闭</a>
                            </span>
                        </div>
                        <div class='login-input-content'>
                            <div class='login-input'>
                                <label>用户名：</label>
                                <input type='text' onkeyup="this.value=this.value.replace(/[^\a-\z\A-\Z0-9]/g,'');" placeholder='请输入用户名' name='username' id='username' class='list-input'>
                            </div>
                            <div class='login-input'>
                                <label>登录密码：</label>
                                <input type='password' onkeyup="this.value=this.value.replace(/[^\a-\z\A-\Z0-9]/g,'');" placeholder='请输入登录密码' name='password' id='password' class='list-input'>
                            </div>
                        </div>
                        <div id='loginBtn' class='login-button'>
                            <a href='javascript:void(0);' id='login-button-submit'>登录</a>
                        </div>
                    </div>
                    <!-- 遮盖层 -->
                    <div id='bg' class='login-bg'></div>
            </div>
            <!-- 内容左边部分 -->
            <div class="con-left-duo">
                <div class="con-left">
                </div>
                <div class="M-box1 m-style">
                </div>
            </div>
            <!-- 内容右边部分 -->
            <div class="con-right">
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Box',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#box{
    width: 1140px;
    /* height: 2000px; */
    margin: 0 auto;
    background-color: antiquewhite;
}

/* 主要内容 */
#box .content{
    width: 1140px;
    height: 900px;
}
/* 主要内容左边部分 */
#box .content .con-left-duo{
    width: 850px;
    height: 900px;
    display: inline-block;
}
#box .content .con-left{
    width: 850px;
    height: 860px;
    display: inline-block;
}
#box .content .con-left .con-left-con{
    width: 100%;
    height: 200px;
    margin-top: 10px;
    box-shadow: 1px 1px 1px #999;
    border-radius: 10px;
}
#box .content .con-left .con-left-con:hover{
    background-color: bisque;
}
#box .content .con-left .con-left-con-a{
    display: block;
    width: 100%;
    height: 200px;
    color: #000000;
}
#box .content .con-left .con-left-con .con-left-top{
    height: 40px;
}
#box .content .con-left .con-left-con .con-left-top-title{
    display: inline-block;
    font-size: 28px;
    padding-left: 20px;
    line-height: 40px;
}
#box .content .con-left .con-left-con .con-left-top-author{
    display: inline-block;
    float: right;
    padding-top: 20px;
    padding-right: 20px;
    color: darkgrey;
    font-size: 12px;
}
#box .content .con-left .con-left-con .con-left-mid{
    height: 120px;
}
#box .content .con-left .con-left-con .con-left-mid-desc{
    padding-top: 10px;
    padding-left: 20px;
    padding-right: 20px;
}
#box .content .con-left .con-left-con .con-left-bot{
    height: 40px;
    line-height: 40px;
}
#box .content .con-left .con-left-con .con-left-bot .con-left-bot-cate{
    display: inline-block;
    padding-left: 20px;
}
#box .content .con-left .con-left-con .con-left-bot .con-left-bot-like{
    display: inline-block;
    float: right;
    padding-right: 20px;
    font-size: 14px;
}

/* 主要内容右边部分 */
#box .content .con-right{
    display: inline-block;
    width: 290px;
    height: 900px;
    float: right;
}
#box .content .con-right .con-right-div{
    width: 98%;
    height: 140px;
    background-color: aliceblue;
    margin-top: 10px;
    margin-left: 3px;
    box-shadow: 3px 3px 2px #999;
    border-radius: 10px;
}
#box .content .con-right .con-right-div:hover{
    /* cursor: pointer; */
    background-color: #f0f1f2;
}
#box .content .con-right .con-right-div p{
    padding-left: 20px;
}
#box .content .con-right .con-right-div p a{
    color: rgb(26, 24, 24);
}
#box .content .con-right .con-right-div .chayu-div{
    margin-top: 10px;
    padding-left: 30px;
}
#box .content .con-right .con-right-div .chayu-div a{
    color: #999;
    font-size: 14px;
}

#clear {
    clear: both;
}

/* 登陆注册部分 */
/*页面登录隐藏区域样式*/

#coverGo .login-header {
    width: 100%;
    text-align: center;
    height: 30px;
    font-size: 24px;
    line-height: 30px;
}

#coverGo .login {
    width: 512px;
    height: 280px;
    position: absolute;
    border: #ebebeb solid 1px;
    left: 50%;
    right: 50%;
    background: #ffffff;
    box-shadow: 0px 0px 20px #ddd;
    z-index: 9999;
    margin-left: -256px;
    margin-top: 140px;
    display: none;
}

#coverGo .login-title {
    width: 100%;
    margin: 10px 0px 0px 0px;
    text-align: center;
    line-height: 40px;
    height: 40px;
    font-size: 18px;
    position: relative;
    cursor: move;
    -moz-user-select: none;
    /*火狐*/
    -webkit-user-select: none;
    /*webkit浏览器*/
    -ms-user-select: none;
    /*IE10*/
    -khtml-user-select: none;
    /*早期浏览器*/
    user-select: none;
}

#coverGo .login-input-content {
    margin-top: 20px;
}

#coverGo .login-button {
    width: 50%;
    margin: 30px auto 0px auto;
    line-height: 40px;
    font-size: 14px;
    border: #ebebeb 1px solid;
    text-align: center;
}

#coverGo .login-bg {
    width: 100%;
    height: 100%;
    position: fixed;
    top: 0px;
    left: 0px;
    background: #000000;
    filter: alpha(opacity=30);
    -moz-opacity: 0.3;
    -khtml-opacity: 0.3;
    opacity: 0.3;
    display: none;
}

#coverGo a {
    text-decoration: none;
    color: #000000;
}

#coverGo .login-button a {
    display: block;
}

#coverGo .login-input input.list-input {
    float: left;
    line-height: 35px;
    height: 35px;
    width: 350px;
    border: #ebebeb 1px solid;
    text-indent: 5px;
}

#coverGo .login-input {
    overflow: hidden;
    margin: 0px 0px 20px 0px;
}

#coverGo .login-input label {
    float: left;
    width: 90px;
    padding-right: 10px;
    text-align: right;
    line-height: 35px;
    height: 35px;
    font-size: 14px;
}

#coverGo .login-title span {
    position: absolute;
    font-size: 12px;
    right: -20px;
    top: -30px;
    background: #ffffff;
    border: #ebebeb solid 1px;
    width: 40px;
    height: 40px;
    border-radius: 20px;
}

#box .header .header-right{
    float: right;
    line-height: 50px;
    margin-top: 15px;
    margin-right: 5px;
    width: 110px;
    height: 50px;
    /* background-color: red; */
    text-align: center;
}
#box .header .header-right .subZhu li {
    display: block;
    height: 40px;
    width: 50px;
    float: right;
    text-align: center;
    margin-top: 5px;
    border-radius: 20px;
    /* margin-left: 10px; */
    background-color: rgb(237, 49, 68);
}

/* 登录后显示相关内容样式 */
#box .header-right .head-mess{
    margin-top: -19px;
    margin-left: 15px;
    position: absolute;
    width: 80px;
    height: 200px;
    /* border: 1px solid red; */
    background-color: #fff;
    z-index: 9999;
    display: none;
    font-size: 14px;
}
#box .header-right .head-mess a{
    color: #5f5f5f
}
</style>
