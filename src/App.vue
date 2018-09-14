<template>
  <div id="app">
    <!-- 顶部 -->
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
        </div>
    <router-view/>
<!-- 底部 -->
        <div class='bottom'>
                <div class='bannerd'>
                    <div class='bannerdt'>
                        <div class='banttt bant1'>
                            <a href='javascript:void(0);'>
                                <h1>
                                    <img src='foot.png' />
                                </h1>
                            </a>
                        </div>
                        <div class='banttt bant2'>
                            <div class='lianjie1'>
                                <ul>
                                    <li>
                                        <a href='javascript:void(0);'>关于我们</a>|</li>
                                    <li>
                                        <a href='javascript:void(0);'>AI相关</a>|</li>
                                    <li>
                                        <a href='javascript:void(0);'>合作申请</a>|</li>
                                    <li>
                                        <a href='javascript:void(0);'>意见反馈</a>
                                    </li>
                                </ul>
                            </div>
                            <div class='shenhe'>
                                <span>由本人亲制</span> 待审核
                            </div>
                        </div>
                        <div class='banttt bant3'>
                            <div class='guanzhu'>
                                <div class='guanwo'>关注我们：</div>
                                <img :src="footImg" alt=''>
                            </div>
                        </div>
                    </div>
                    <div class='bannerdb'>
                        <div class='banndbt'>
                            <div class='zzz'>友情链接：</div>
                            <ul>
                                <li>
                                    <a href='javascript:void(0);'>伞兵小队</a>|
                                </li>
                                <li>
                                    <a href='javascript:void(0);'>壮哉104</a>|
                                </li>
                                <li>
                                    <a href='javascript:void(0);'>都会成为老男孩</a>|
                                </li>
                                <li>
                                    <a href='javascript:void(0);'>D350</a>|
                                </li>
                                <li>
                                    <a href='javascript:void(0);'>大邳</a>|
                                </li>
                                <li>
                                    <a href='javascript:void(0);'>站长之家</a>
                                </li>
                                <li>
                                    <a href='admin/index/login.html'>管理员</a>
                                </li>
                            </ul>
                        </div>
                        <div class='banndbb'>
                            Powered by Sanbing v1.0.0 &copy;2017 伞兵一队
                        </div>
                    </div>
                </div>
                <div id='clear'></div>
        </div>
  </div>
</template>

<script>
import footImg from './assets/index/foot.png'
export default {
  name: 'App',
  date () {
    return {
      footImg: footImg
    }
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  list-style:none;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}
/* 头部的样式 */
.header {
    width: 1140px;
    height: 80px;
    margin: 0 auto;
    /* background-color: aquamarine; */
    /* background: url("head.png") no-repeat; */
    background-size: 100%;
}
/* 头部左边导航栏 */
.header .header-left li{
    height: 40px;
    width: 80px;
    float: left;
    text-align: center;
    margin-left: 100px;
    margin-top: 19px;
    background-color: #ED7D31;
    border: 1px solid #ED7D31;
    border-radius: 20px;
}
.header .header-left li a {
    display: block;
    height: 40px;
    width: 80px;
    line-height: 40px;
    color: darkslategrey;
}

.header .header-left li:hover {
    background-color: #ED7D31;
    /* border-radius: 50%; */
}
.header .header-left li:nth-child(1) {
    margin-left: 0;
}
.header .header-left li:last-child{
    background-color: gainsboro;
}
.header .header-left li:hover{
    background-color: #f0f1f2;
}
.header .header-right .subZhu li a {
    display: block;
    height: 40px;
    width: 50px;
    line-height: 40px;
}

.header .header-right .subZhu li a:active {
    color: blue;
}

.header .header-right .subZhu li:nth-child(2) {
    margin-right: 5px;
}
/* 底部样式 */
.bottom {
    width: 100%;
    background-color: #515151;
    margin-top: 10px;
}

.bottom .bannerd {
    width: 1140px;
    margin: 0 auto;
}

.bottom .bannerd .bannerdt {
    height: 127px;
    width: 100%;
    border-bottom: 1px solid #5f5f5f;
}

.bottom .bannerd .bannerdt .banttt {
    width: 300px;
    height: 55px;
    float: left;
    margin-left: 60px;
    margin-top: 37px;
}

.bottom .bannerd .bannerdt .bant1 img {
    margin-top: -20px;
    border-radius: 50px;
}

.bottom .bannerd .bannerdt .bant2 li {
    float: left;
    font-size: 14px;
    color: #fff;
    font-size: 14px;
    margin-left: 10px;
}

.bottom .bannerd .bannerdt .bant2 li:first-child {
    margin-left: 0;
}

.bottom .bannerd .bannerdt .bant2 a {
    color: #fff;
    margin-right: 10px;
}

.bottom .bannerd .bannerdt .bant2 li:last-child a {
    margin-right: 0;
}

.bottom .bannerd .bannerdt .bant2 .shenhe {
    float: left;
    font-size: 12px;
    color: #999;
    width: 300px;
    text-align: center;
    margin-top: 10px;
}

.bottom .bannerd .bannerdt .bant2 .shenhe span {
    margin-right: 23px;
}

.bottom .bannerd .bannerdt .bant3 {
    line-height: 55px;
    margin-left: 120px;
}

.bottom .bannerd .bannerdt .bant3 .guanwo {
    float: left;
    color: #fff;
}

.bottom .bannerd .bannerdt .bant3 .guanzhu img {
    width: 127px;
    margin-top: -37px;
    margin-left: 40px;
}

.bottom .bannerd .bannerdb {
    height: 73px;
    width: 100%;
    font-size: 12px;
    color: #999;
    margin-top: 16px;
}

.bottom .bannerd .bannerdb .banndbt a {
    margin-right: 18px;
    color: #999;
}

.bottom .bannerd .bannerdb .banndbt .zzz {
    float: left;
    margin-left: 60px;
}

.bottom .bannerd .bannerdb .banndbt li {
    float: left;
    margin-left: 18px;
}

</style>
