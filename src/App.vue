<template>

<header id="header" class="clear">
    <div id="gameLogo"><a href="#"><img src="./assets/imges/gameLogo.png" alt=""></a></div>
    <div class="gameIndex"><a href="#">首页</a></div>
    <div id="menu">
        <a href="#">注册</a> |
        <a href="#">登录</a> |
        <a href="#">帮助</a> |
        <a href="#">更多</a>

    </div>
</header>
<!-- 主体 -->
<article id="container">
    <!-- 左边 -->
    <section class="gameLeft">
        <div class="clear firstLine">
            <div class="gameNav">
                <ul>
                    <li v-for="(item,index) in gameList1" :key="index" >
                    <img :src="item.pic" style="padding:0px 10px 0px 10px" >{{item.name}}
                    <img :src="item.pic2" style="position:absolute;right:15px top: 5px;" >
                </li>
                </ul>
            </div>
            <div class="gameAdver"><a href="#"><img src="./assets/imges/xdtgg_frxz2_44.jpg" ></a>
                <ul class="code clear">
                    <li class="active"><a href="#">1</a></li>
                    <li><a href="#"></a>2</li>
                    <li><a href="#"></a>3</li>
                    <li><a href="#"></a>4</li>
                </ul>
            </div>
        </div>
        <div class="qb">
            <div class="top">
                <dl>
                    <dt>全部游戏</dt>
                    <dd><a href="#">战争策略</a></dd>
                    <dd>|</dd>
                    <dd><a href="#">体育经营</a></dd>
                    <dd>|</dd>
                    <dd><a href="#">社交游戏</a></dd>
                </dl>
            </div>
           
            <div class="allGame">
                <ul class="clear">
                    <li v-for="(item,index) in gameList0" :key="index">
                        <div class="img">
                            <a href="#">
                                <img :src="item.pic11">
                            </a>
                        </div>
                        <div class="list">
                            <p>{{item.dsb}}</p>
                            <p>{{item.dsb1}}</p>
                            <p>{{item.dsb2}}<span style="color: rgb(color: #a70a0a;);">{{item.dsb0}}</span></p>
                            <p class="playBtn"><a href="">{{item.dsb3}}</a><a class="active" href="#">{{item.dsb4}}</a></p>
                        </div>
                    </li>
                   
                </ul>    
            </div>
        </div>
        <div class="gameBorder" style="position: absolute;top: 550px;">
            <div class="top">
                <dl>
                    <dt>角色扮演</dt>
                </dl>
            </div>
            <div class="role">
                <ul>
                    <li v-for="(item,index) in gameList2" :key="index">
                        <img :src="item.pic3">
                        <p>{{item.ccg2}}</p>
                        <p>{{item.ccg3}}<span style="color:rgb(color: #a70a0a;);">{{item.ccg5}}</span></p>
                        <p></p>
                        <p class="playBtn"><a href="">{{item.ccg4}}</a><a class="active" href="#">{{item.ccg6}}</a></p>
                        <span style="color: red;"></span>
                    </li>
                </ul>
 
            </div>
            

        </div>
    </section>
    <aside class="gameRight">
        <div class="gameLogin clear">
            <h1>开心网用户登录</h1>

            <form action="#">
                <ul>
                    <li>账号：
                        <input name="username" type="text" placeholder="字母、数字的六位字符" required/>
                    </li>
                    <li>密码：
                        <input name="pwd" type="password" placeholder="四位数字" required/>
                    </li>
                    <li>
                        <input class="login" name="login" type="submit" value=" "/>

                    </li>
                    <li>
                        <a href="#">立即注册</a>
                        <a href="#">忘记密码</a>
                    </li>
                </ul>
            </form>

        </div>
         <div class="gameBorder"  style="position:0;">
            <div class="top" >
                <dl>
                    <dt>新闻公告</dt>
                </dl>
            </div>
            <ul class="news">
                <li v-for="(item,index) in gamenews" :key="index">
                    <img :src="item.newpic250" ><a href="#">{{item.new1}}</a>
                
                
                </li>
            </ul>
         </div>
         <div class="ad">
            <a href="#"><img src="./assets/imges/ad1.jpg" /></a>
            <a href="#"><img src="./assets/imges/ad2.jpg" /></a>
        </div>
        <div class="gameBorder">
        <div class="top">
            <dl>
                <dt>游戏视频</dt>
            </dl> 
        </div>
        <div class="clear">
            <dl class="gameVideo">
                <dt v-for="(item,index) in gameVideo" :key="index">
                    <img :src="item.video" >
                    <a href="#">{{item.ccf}}</a>
                    
                </dt>
                
            </dl>
        </div>

    </div>
        </aside>
    <div>
       <div class="head" ></div>
    </div>
    
</article>
<footer id="footer">
    <a href="#">关于我们</a>
    <a href="#">手机版</a>
    <a href="#">开放平台</a>
    <a href="#"> 自助广告</a>
    <a href="#"> 招聘</a>
    <a href="#">客服</a>
    <a href="#">帮助</a>
    @2017开心网&nbsp;&nbsp; 文网文[2009]157号&nbsp;&nbsp; 京ICP证080482号&nbsp;&nbsp; 京公网安备110000000003号 未成年人家长监护
</footer>
<div class="adRight">
    <a class="icon" href="#">X</a>
    <a href="#"><img src="./assets/imges/ad3.jpg" alt=""/></a>
</div>

</template>

<style>
/*漂浮广告2*/

.icon2 {
    position: absolute;
    right: 0;
    top: -12px;
    background: rgba(204, 204, 204, 0.63);
    padding: 0 4px;
}
.adRight2 img {
    width: 100%;
}
@keyframes adv {
    0% {
        right: 0;
        top: 0;
    }
    50% {
        right: 800px;
        top: 700px;
    }
    100% {
        right: 0;
        top: 400px;
    }
}
    .qb{
        width: 724px;
        height: 223px;
        position: absolute;
        top: 300px;
        border: 1px solid rgba(128,128,128,0.4);
    }
    .top{
        width: 100%;
       height: 35px ;
        background: linear-gradient(to bottom, #fafafa, #fafafa, #f6f7f6, #f5f4f4, #f3f4f3, #f1f2f1, #eeefef);
    }
    .qb dl{
        display: flex;
        flex-direction: row;
        position: absolute;
        top: 5px;
    }
</style>

<script>
export default{
    data() {
        return {
            gameList0:[{pic11:require("./assets/imges/img-4.jpg"),dsb:"三国题材横版RPG网游,丰富的武将系统",dsb1:"类型：角色扮演",dsb2:"游戏人气 :",dsb0:"470921",dsb3:"选服",dsb4:"进入游戏"}
                    ,{pic11:require("./assets/imges/img-5.jpg"),dsb:"一款不建主城不等CD,不占资源，全程战斗",dsb1:"类型：战征策略",dsb2:"游戏人气 :8745221",dsb3:"选服",dsb4:"进入游戏"}, ],
            gameList1:[
            {pic:require("./assets/imges/sub-2.gif"),name:"征战四方",pic2:require("./assets/imges/rightA.png")},
            {pic:require("./assets/imges/sub-3.gif"),name:"龙将",pic2:require("./assets/imges/rightA.png")},
            {pic:require("./assets/imges/sub-4.gif"),name:"弹弹堂",pic2:require("./assets/imges/rightA.png")},
            {pic:require("./assets/imges/sub-5.gif"),name:"凡人修真2",pic2:require("./assets/imges/rightA.png")},
            {pic:require("./assets/imges/sub-6.gif"),name:"一骑当先",pic2:require("./assets/imges/rightA.png")},
            {pic:require("./assets/imges/sub-7.gif"),name:"宫廷计",pic2:require("./assets/imges/rightA.png")},
            {pic:require("./assets/imges/sub-8.gif"),name:"神仙道",pic2:require("./assets/imges/rightA.png")},],
            gameList2:[
            {pic3:require("./assets/imges/img-6.jpg"),ccg2:"游戏人气 :1765314",ccg3:"游戏状态 :",ccg4:"选服",ccg5:"22区开启",ccg6:"进入游戏"},
            {pic3:require("./assets/imges/img-7.jpg"),ccg2:"游戏人气 :1245814",ccg3:"游戏状态 :",ccg4:"选服",ccg5:"23区开启",ccg6:"进入游戏"},
            {pic3:require("./assets/imges/img-8.jpg"),ccg2:"游戏人气 :1245814",ccg3:"游戏状态 :",ccg4:"选服",ccg5:"25区开启",ccg6:"进入游戏"},
            {pic3:require("./assets/imges/img-9.jpg"),ccg2:"游戏人气 :123745", ccg3:"游戏状态 :",ccg4:"选服",ccg5:"18区开启",ccg6:"进入游戏"},
            {pic3:require("./assets/imges/img-10.jpg"),ccg2:"游戏人气 :178501",ccg3:"游戏状态 :",ccg4:"选服",ccg5:"火爆开启",ccg6:"进入游戏"},
            {pic3:require("./assets/imges/img-11.jpg"),ccg2:"游戏人气 :983014",ccg3:"游戏状态 :",ccg4:"选服",ccg5:"2区开启",ccg6:"进入游戏"},
            {pic3:require("./assets/imges/img-12.jpg"),ccg2:"游戏人气 :745214",ccg3:"游戏状态 :",ccg4:"选服",ccg5:"4区开启",ccg6:"进入游戏"},
            {pic3:require("./assets/imges/img-13.jpg"),ccg2:"游戏人气 :654814",ccg3:"游戏状态 :",ccg4:"选服",ccg5:"火爆开启",ccg6:"进入游戏"},
        ],
        gamenews:[
        {newpic250:require("./assets/imges/rightTwo.png"), new1:"[征战四方] 开心首服·黄巾之乱"},
        {newpic250:require("./assets/imges/rightTwo.png"), new1:"[龙将] 火爆8服·八门金"},
        {newpic250:require("./assets/imges/rightTwo.png"), new1:"[弹弹堂] 41服开启·万人竞技"},
        {newpic250:require("./assets/imges/rightTwo.png"), new1:"[凡人修真2] 03月08日·四海帝王"},
        {newpic250:require("./assets/imges/rightTwo.png"), new1:"[一骑当先] 开心2服上线送黄金"},
        {newpic250:require("./assets/imges/rightTwo.png"), new1:"[宫廷计] 03月06日·西施秘史"},
        {newpic250:require("./assets/imges/rightTwo.png"), new1:"[凡人修真2] 03月08日·四海帝王"},
         ],
         gameVideo:[
         {video:require("./assets/imges/img-1.jpg"),ccf:"航海之王》麻辣炫酷反穿越，英雄时尚大变身！"},
         {video:require("./assets/imges/img-2.jpg"),ccf:"《弹弹堂》吴克群同名激情主题MV,体验修真乐趣！"},
         ]

      

            
        }
    },
}



</script>


<style>
body {
    font-family: Verdana, Arial, Helvetica, sans-serif, "宋体";
    line-height: 20px;
    font-size: 12px;
}
*{
    margin: 0 ;
    padding: 0;
}
li {
    list-style: none;
}
#container, #footer, #header {
    width: 1000px;
    margin: 0 auto;
    overflow: hidden;
    clear: both;
}
a img {
    border: 0;
}
a {
    text-decoration: none;
    color: #2b62a5;
}
/* 页面顶部样式 */
#header{
    height: 50px;
    background:linear-gradient(to bottom,#d01d3b, #d3617a);
    margin-bottom: 20px;
    border-radius: 8px;
}
#menu {
    float: right;
    color: #dbb9b9;
    padding: 15px 30px 0 0;
}
#menu a {
    color: #ffffff;
    padding: 0 5px;
}
/*鼠标移入字体放大*/
#menu a:hover {
    transform: scale(3);
    -webkit-transform: scale(3);
    -moz-transform: scale(3);
    -o-transform: scale(3);
    font-weight: bold;
    text-decoration: none;
}
/*网页游戏页面样式*/
#gameLogo {
    float: left;
    padding-top: 5px;
}
.gameIndex{
    background: url(./assets/imges/btn-01.gif) 0 0 no-repeat;
    width: 100px;
    height: 40px;
    text-align: center;
    float: left;
    position: relative;
    left: 20px;
    top: 10px;
}
.gameIndex a, .gameIndex a:hover {
    font-size: 14px;
    color: #cb3333;
    text-decoration: none;
    font-weight: bold;
    line-height: 40px;
}
/* 左 */
.gameLeft {
    float: left;
    width: 724px;
    overflow: hidden;
}
.firstLine {
    margin-bottom: 20px;
}
.gameNav {
    float: left;
    border: 1px #cb3333 solid;
    border-radius: 8px;
    overflow: hidden;
    width: 190px;
}
.gameNav li {
    background: linear-gradient(to bottom, #ffffff, #f8f8f8, #e8e8e8, #eaeaea, #f1eff0);
    line-height: 30px;
}
.gameNav li img {
    padding: 0 10px 0 8px;
    vertical-align: middle;
}
.gameNav li a {
    color: #000000;
    display: block;
    width: 190px;
    height: 27px;
    padding-top: 2px;
    background: url("./assets/imges/rightA.png") 170px center no-repeat;
}
.gameNav li:hover {
    color: #fff;
    text-decoration: none;
    background: linear-gradient(to right, #ff0000, #f6ff00, #0043b6, #00e50b, #00bda4, #eb0099, #dd00ff);
}
.gameAdver {
    float: right;
    overflow: hidden;
    width: 520px;
    position: relative;
    margin-top: 4px;
}
.gameAdver img {  
    width: 100%;
    border-radius: 8px;
}
.code {
    position: absolute;
    bottom: 10px;
    right: 30px;
}
.code li {
    float: left;
    padding: 0 6px;
    background: rgba(204, 204, 204, 0.98);
    margin: 4px;
    border-radius: 50%;
}
.code .active {
    background: rgba(166, 1, 86, 0.98);
}
.code .active a {
    color: #fff;
}
.code li a {
    color: #000;
}
.allGame {
    padding: 20px;
    border-bottom: 1px #cccccc solid;
    border-radius: 8px;
    width: 672px;
    overflow: hidden;
}

.allGame li {
    width: 320px;
    height: 130px;
    overflow: hidden;
    border: 1px #cccccc solid;
    border-radius: 8px;
    float: left;
    margin-left: 8px;
    padding: 10px 0;

}

.allGame li .img {
    float: left;
    width: 128px;
    box-sizing: border-box;
    margin: 10px 10px 0 8px;
}

.allGame li .img img {
    width: 100%;
}

.allGame li .list {
    float: right;
    width: 174px;
}

/*左边栏里的游戏列表的图片鼠标移入发生动画*/
.img img, .role img {
    transition: all 0.5s;
}

.img img:hover, .role img:hover {
    transform: translate(-8px, 0);
}

.allGame p {
    line-height: 22px;
}

.allGame span {
    color: #a70a0a;
}

.playBtn {
    margin-top: 4px;
}

.playBtn a {
    height: 26px;
    line-height: 26px;
    display: inline-block;
    padding: 0 10px;
    border: 1px solid #c7c9cf;
    border-radius: 4px;
    color: #333333;
}

.playBtn .active {
    background: linear-gradient(to bottom, #87c9d9, #69b2c8, #5b9dbc, #4a87ac, #3e74a2, #396f9e, #366b9b);
    color: #fff;
    font-weight: bold;
    border: 1px solid #326598;
    margin-left: 4px;
}

.role {
    width: 680px;
    overflow: hidden;
    clear: both;
    margin: 15px auto 0;
}

.role li {
    float: left;
    width: 170px;
    text-align: center;
    height: 190px;
    overflow: hidden;
}

.role h1 {
    font-size: 14px;
    line-height: 30px;
    text-align: center;
}

.role h1 a, .role h1 a:hover {
    color: #a70a0a;
}

.role p span {
    color: #a70a0a;
}

.gameRight {
    float: right;
    width: 262px;
    overflow: hidden;
}

.gameLogin {
    border: 1px #cccccc solid;
    border-radius: 8px;
    height: 206px;
    overflow: hidden;
    background-color: rgba(243, 243, 243, 0.46);
    margin-bottom: 20px;
}

.gameLogin h1 {
    color: #767373;
    font-size: 14px;
    padding: 20px 0px 25px 20px;
}

.gameLogin li {
    padding-left: 20px;
    height: 35px;
    font-size: 14px;
}

.gameLogin li input {
    border: 1px #cccccc solid;
    width: 150px;
    height: 20px;
    padding-left: 8px;
}

.gameLogin .login {
    background: url(./assets/imges/btnLogin.jpg) 0 0 no-repeat;
    width: 63px;
    height: 24px;
    cursor: pointer;
    border: 0;
    margin-left: 80px;
    margin-bottom: 20px;
}

.gameLogin li a {
    margin-left: 30px;
}

.gameLogin li a:hover {
    text-decoration: underline;
}

.gameBorder {
    border: 1px #cccccc solid;
    border-radius: 8px;
    margin-bottom: 20px;
    width: 724px;
}

.top dt {
    font-size: 14px;
    font-weight: bold;
    color: #7d0808;
    padding-left: 10px;
    padding-right: 30px;
    line-height: 28px;
    float: left;
}
.top dd {
    float: left;
    color: #cccccc;
    padding: 0px 5px;
    line-height: 28px;
}

.top dd a {
    color: #666666;
    font-size: 14px;
}
/* 新闻栏， */
.news {
    width: 95%;
    margin: 0 auto;
}

.news li {
    border-bottom: 1px #cccccc dashed;
    height: 27px;
    
    padding-left: 45px;
    line-height: 27px;
    /*制作过渡动画*/
    transition: all 0.5s;
    -webkit-transition: all 0.5s;
    -moz-transition: all 0.5s;
    -o-transition: all 0.5s;
}
/*制作鼠标移入新闻公告列表时，产生文字向上移动，放大的动画*/
.news li:hover {
    transform: translate(0, 4px) scale(1.1);
    -webkit-transform: translate(0, 4px) scale(1.1);
    -moz-transform: translate(0, 4px) scale(1.1);
    -o-transform: translate(0, 4px) scale(1.1);
}

.news .noBorder {
    border-bottom: 0;
}

.news li a {
    color: #4d4646;
}
.ad {
    margin-bottom: 10px;
}

.ad img {
    width: 98%;
    margin: 5px;
}
.gameVideo {
    width: 95%;
    margin: 0px auto;
    line-height: 26px;
}

.gameVideo dt {
    border-bottom: 1px #cccccc dashed;
    clear: both;
    width: 100%;
    overflow: hidden;
    padding: 10px 0px;
}

.gameVideo dd {
    clear: both;
    width: 100%;
    overflow: hidden;
    padding: 10px 0px;
}

.gameVideo img {
    padding: 0px 10px 0px 0px;
    float: left;
}
/*页面底部样式*/
#footer {
    padding: 15px 0;
    clear: both;
    text-align: right;
    color: #666666;
}

#footer a {
    padding-right: 15px;
    float: left;
}

.footerBorder-top {
    border-top: 1px #cccccc solid;
}
/*漂浮广告*/
.adRight {
    width: 200px;
    position: absolute;
    right: 0;
    top: 400px;
    animation: ad 3s both;
}
.icon {
    position: absolute;
    right: 0;
    top: -12px;
    background: rgba(204, 204, 204, 0.63);
    padding: 0 4px;
}
.adRight img {
    width: 100%;
}
@keyframes ad {
    0% {
        right: 0;
        top: 0;
    }
    50% {
        right: 800px;
        top: 700px;
    }
    100% {
        right: 0;
        top: 400px;
    }
}

















</style>