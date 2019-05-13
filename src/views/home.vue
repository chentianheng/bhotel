<template>
<div id="container" >
    <div id="banner" class="bannerImg">
        <h1>微信生态+PC网页端</h1>
        <h1>一体化酒店智慧营销管理解决方案</h1>
        <h2>助力粉丝留存，增加酒店收入。</h2>
        <a href="#">免费试用30天</a>
    </div>
    <header class="headerContainer">
        <div class="header">
            <i>
                <img src="../assets/logo.png" alt="logo" >
            </i>
            <nav>
                <ul>
                    <li><a href="#">首页</a></li>
                    <li><a href="#">解决方案</a></li>
                    <li><a href="#">关于我们</a></li>
                    <li><a href="#">联系我们</a></li>
                    <li><a href="#">English</a></li>
                </ul>
            </nav>
        </div>
    </header>
    <div class="dashboardContainer">
        <h1>一站式满足酒店后端管理需求</h1>
        <div class="dashboard">
            <div class="item">
                <i><img src="../assets/icon/calendar.png" alt="calendar"></i>
                <h1>房价日历</h1>
                <h2>支持根据不同时间制定房价</h2>
            </div>
            <div class="item">
                <i><img src="../assets/icon/luggage.png" alt="luggage"></i>
                <h1>入住/退房管理</h1>
                <h2>快速办理客户入住以及可提前退房</h2>
            </div>
            <div class="item">
                <i><img src="../assets/icon/branch.png" alt="branch"></i>
                <h1>客房分配</h1>
                <h2>帮助前台进行客房及时分配</h2>
            </div>
        </div>
        <div class="dashboard">
                <div class="item">
                    <i><img src="../assets/icon/status.png" alt="status"></i>
                    <h1>房态标记</h1>
                    <h2>快速的查看、修改房间状态</h2>
                </div>
                <div class="item">
                    <i><img src="../assets/icon/data.png" alt="data"></i>
                    <h1>数据管理</h1>
                    <h2>经营数据记录以及深入分析</h2>
                </div>
                <div class="item">
                    <i><img src="../assets/icon/hotel.png" alt="hotel"></i>
                    <h1>多门店管理</h1>
                    <h2>连锁型酒店全门店统一管理</h2>
                </div>
        </div>
    </div>
    <div class="productContainer">
        <div class="left">
            <img src="../assets/wechatDash.png" alt="wechatDash" width="650">
        </div>

        <!--切换不同的产品，并且有不同的样式效果-->
        <div id="productCard" class="right">
                <a href="#"
                   v-bind:class="{ productCardActive : P1IsActive , productCard : P1NoActive}"
                   @mouseenter="enterP1"
                   @mouseleave="leaveP1"
                >
                    <i class="productCardIcon"><img src="../assets/icon/PC.png" alt="公众号+PC"></i>
                    <div class="productCardContainer">
                        <h1 class="productCardIconTitle">公众号+PC官网</h1>
                        <h2 class="productCardIconSub">包含官网的完整生态</h2>
                        <!--动画效果箭头-->
                        <transition name="fade">
                            <div class="P1Enter"
                                 v-show="P1arrowShow"
                            ><img src="../assets/icon/P1Enter.png" alt="进入键" >
                            </div>
                        </transition>
                        <!--动画三角形-->
                        <transition name="triangle-fade">
                        <div class="triangle"
                             v-show="P1triangleShow"></div>
                        </transition>
                    </div>
                </a>

            <a href="#"
               v-bind:class="{ productCardActive : P2IsActive , productCard : P2NoActive}"
               @mouseenter="enterP2"
               @mouseleave="leaveP2"
            >
                <i class="productCardIcon"><img src="../assets/icon/service.png" alt="公众号+管理后台"></i>
                <div class="productCardContainer">
                    <h1 class="productCardIconTitle">公众号+管理后台</h1>
                    <h2 class="productCardIconSub">能满足大部分酒店的运作需求</h2>
                    <!--动画效果箭头-->
                    <transition name="fade">
                        <div class="P2Enter"
                             v-show="P2arrowShow"
                        ><img src="../assets/icon/P2Enter.png" alt="进入键" >
                        </div>
                    </transition>
                    <!--动画三角形-->
                    <transition name="triangle-fade">
                        <div class="P2triangle"
                             v-show="P2triangleShow"></div>
                    </transition>
                </div>
            </a>

            <a href="#"
               v-bind:class="{ productCardActive : P3IsActive , productCard : P3NoActive}"
               @mouseenter="enterP3"
               @mouseleave="leaveP3"
            >
                <i class="productCardIcon"><img src="../assets/icon/miniProgram.png" alt="小程序"></i>
                <div class="productCardContainer">
                     <h1 class="productCardIconTitle">小程序+管理后台</h1>
                     <h2 class="productCardIconSub">最新解决方案，更好的体验</h2>
                    <!--动画效果箭头-->
                    <transition name="P3-fade">
                        <div class="P3Enter"
                             v-show="P3arrowShow"
                        >即将推出
                        </div>
                    </transition>
                    <!--动画三角形-->
                    <transition name="triangle-fade">
                        <div class="P3triangle"
                             v-show="P3triangleShow"></div>
                    </transition>
                </div>
            </a>
        </div>
    </div>
    <div class="impressionContainer">
        <div class="impression">
            <h1>合作伙伴评价</h1>
            <div class="content">
                <p>贵公司诚实可信，业务水平强，为客户着想，办客户未想到的事情，主动为客户服务。愿你公司继续保持，不忘初心。祝2019心想事成，财运亨通！</p>
            </div>
            <div class="customer">
                <i><img src="../assets/Huang.png" alt="Mr.Huang"></i>
                <div class="info">
                    <h1>黄总</h1>
                    <p>多伦多连锁酒店</p>
                </div>
            </div>
        </div>
    </div>
    <div class="hotelContainer">
        <div class="left"></div>
        <div class="right">
            <h1>深圳多伦多连锁酒店</h1>
            <p>深圳多伦多连锁酒店目前拥有12家分店，并将计划在2019年继续拓展他们的商业版图。</p>
            <p>该酒店通过使用我司的管理系统从而达到了留存用户，增加营业额，降低人员管理开支的效果。</p>
            <a href="#">了解更多</a>
        </div>
    </div>
    <div class="marketingContainer">
        <h1>开启智慧营销之路</h1>
        <h2>适用于微信生态+酒店管理的一体式解决方案</h2>
        <img src="../assets/methods.png" alt="methods">
    </div>
    <footer class="footerContainer">
        <div class="contentContainer">
            <div class="footer">

                <!--合作伙伴-->
                <div class="footerList">
                    <h1>合作伙伴</h1>
                    <ul>
                        <li><a href="http://www.dldhotels.com/home"><img src="../assets/icon/dldhotel.png" alt="多伦多连锁酒店"></a></li>
                    </ul>
                </div>

                <!--产品定制-->
                <div class="footerList">
                    <h1>产品定制</h1>
                    <ul>
                        <li><a href="#">小程序</a></li>
                        <li><a href="#">公众号</a></li>
                        <li><a href="#">公司官网</a></li>
                        <li><a href="#">H5页面</a></li>
                        <li><a href="#">数据处理</a></li>
                    </ul>
                </div>

                <!--公司简介-->
                <div class="footerList">
                    <h1>公司</h1>
                    <ul>
                        <li><a href="#">关于我们</a></li>
                        <li><a href="#">工作机会</a></li>
                        <li><a href="#">合作伙伴</a></li>
                    </ul>
                </div>

                <!--其他-->
                <div class="footerList">
                    <h1>其他</h1>
                    <ul>
                        <li>chentianhengg@gmail.com</li>
                        <li><span>+86 155 2102 6970</span></li>
                        <li>周一至周日 9:00 ~ 22:00</li>
                    </ul>
                </div>
            </div>
        </div>
        <p>Copyright © 2019 hotel.bintre.com. All Rights Reserved 深圳市二叉树科技有限公司版权所有 粤ICP备17019238号</p>
    </footer>
</div>
</template>

<script>
    export default {
        el:'#productCard',
        data(){
            return{
                P1IsActive:true,
                P2IsActive:false,
                P3IsActive:false,

                P1NoActive:false,
                P2NoActive:true,
                P3NoActive:true,

                P1arrowShow:false,
                P2arrowShow:false,
                P3arrowShow:false,

                P1triangleShow:true,
                P2triangleShow:false,
                P3triangleShow:false,

            }
        },
        methods:{
            enterP1:function(){
                this.P1IsActive = true;
                this.P2IsActive = false;
                this.P3IsActive = false;

                this.P1NoActive = false;
                this.P2NoActive = true;
                this.P3NoActive = true;

                this.P1arrowShow = true;

                this.P1triangleShow = true;
                this.P2triangleShow = false;
                this.P3triangleShow = false;

            },
            leaveP1:function(){
                this.P1arrowShow = false;
            },
            enterP2:function(){
                this.P1IsActive = false;
                this.P2IsActive = true;
                this.P3IsActive = false;

                this.P1NoActive = true;
                this.P2NoActive = false;
                this.P3NoActive = true;

                this.P2arrowShow = true;

                this.P1triangleShow = false;
                this.P2triangleShow = true;
                this.P3triangleShow = false;
            },
            leaveP2:function(){
                this.P2arrowShow = false;
            },
            enterP3:function(){
                this.P1IsActive = false;
                this.P2IsActive = false;
                this.P3IsActive = true;

                this.P1NoActive = true;
                this.P2NoActive = true;
                this.P3NoActive = false;

                this.P3arrowShow = true;

                this.P1triangleShow = false;
                this.P2triangleShow = false;
                this.P3triangleShow = true;
            },
            leaveP3:function () {
                this.P3arrowShow = false;
            }
        }
    }
</script>

<style scoped>
        /*动画*/
        /*右侧的箭头动画*/

        .fade-enter-active {
            transition: all .4s ease;
        }
        .fade-leave-active{
            transition: all .2s cubic-bezier(1.0,0.5,0.8,1.0);
        }
        .fade-enter,.fade-leave-to{
            transform:translateX(80px);
            opacity: 0;
        }

        /*左侧的箭头动画*/
        .triangle-fade-enter-active {
            transition: all .4s ease;
        }
        .triangle-fade-leave-active{
            transition: all .2s cubic-bezier(1.0,0.5,0.8,1.0);
        }
        .triangle-fade-enter,.triangle-fade-leave-to{
            transform:translateX(20px);
            opacity: 0;
        }
        /*动画结束*/

        /*左侧的箭头动画*/
        .P3-fade-enter-active {
            transition: all .4s ease;
        }
        .P3-fade-leave-active{
            transition: all .2s cubic-bezier(1.0,0.5,0.8,1.0);
        }
        .P3-fade-enter,.P3-fade-leave-to{
            transform:translateX(-60px);
            opacity: 0;
        }
        /*动画结束*/

        /*容器的样式*/
        #container{
            display: flex;
            flex-direction: column;
        }

        /*banner的样式*/
        .bannerImg {
            background-image: url("../assets/banner.png");
            background-repeat: no-repeat;
            background-size: 100%;
            width: 100%;
            height: 600px;
            min-width: 1275px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }

        .bannerImg h1{
            font-family: PingFangSC-Regular,sans-serif;
            color: #FFFFFF;
            font-size: 2.2rem;
            font-weight: 400;
        }

        .bannerImg h2{
            font-family: PingFangSC-Regular,sans-serif;
            color: #FFFFFF;
            margin-top: 10px;
            font-size: 1.2rem;
            font-weight: 400;
        }

        .bannerImg a{
            font-family: PingFangSC-Regular,sans-serif;
            width: 160px;
            height: 50px;
            text-align: center;
            line-height: 50px;
            font-size: 0.9rem;
            text-decoration: none;
            color: #695229;
            font-weight: 500 ;
            background-color: #FFFFFF;
            border-radius: 50px;
            margin-top: 30px;
        }

        .headerContainer {
            display: flex;
            width: 100%;
            height: 80px;
            position: absolute;
            align-items: center;
            justify-content: center;
            min-width: 1270px;
        }

        .header{
            display: flex;
            width: 1270px;
            padding: 0 30px;
            justify-content: space-between;
        }

        .headerContainer i img{
            width: 40px;
        }

        .header ul li{
            list-style: none;
            float: left;
            margin-top: 10px;
        }

        .header ul li a{
            font-family: PingFangSC-Regular,sans-serif;
            text-decoration: none;
            list-style: none;
            float: left;
            color: #FFFFFF;
            margin-left: 10px;

        }

        .header ul li a:hover {
            border-bottom: 2px solid #FFFFFF;
        }

        /*后端需求样式*/
        .dashboardContainer{
            display: flex;
            height: 500px;
            width: 100%;
            align-items: center;
            flex-direction: column;
            min-width: 1270px;
        }

        .dashboardContainer h1{
            font-family: PingFangSC-Regular,sans-serif;
            color: #695229;
            margin: 50px;
            font-size: 1.4rem;
            font-weight: 500;
        }

        .dashboard{
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            width: 55%;
        }

        .dashboard .item{
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .dashboard .item h1{
            font-family: PingFangSC-Regular,sans-serif;
            color: #707070;
            font-size: 1rem;
            margin: 10px ;
        }

        .dashboard .item h2{
            font-family: PingFangSC-Regular,sans-serif;
            color: #707070;
            font-size: 0.8rem;
            margin: 0 0 80px;
            font-weight: 100;
        }

        .dashboard .item  img{
            width: 40px;
            height: 40px;
        }

        /*产品简介栏*/
        .productContainer{
            display: flex;
            min-width: 1270px;

        }

        .productContainer .left{
            display: flex;
            width: 66%;
            height: 600px;
            background: linear-gradient(#CCEDFC, #9FD1F5);
            justify-content: center;
            align-items: center;
        }

        .productContainer .right{
            width: 34%;
            height: 600px;
            background-color: #FFFFFF;
        }


        /*a标签产品卡-未激活状态*/
        .productCard{
            display: flex;
            text-decoration: none;
            color: #000000;
            height: 200px;
            align-items: center;
            opacity: 0.1;
            z-index: 2;
        }

        /*a标签产品卡-激活状态*/
        .productCardActive{
            display: flex;
            text-decoration: none;
            color: #000000;
            height: 198px;
            align-items: center;
            border-left: none;
            box-shadow: 0 0 10px rgba(20,89,193,0.2);
            z-index: 2;

        }

        /*i标签下的img图片*/
        .productCardIcon img{
            width: 80px;
            margin-left: 60px;
        }

        .productCardIconTitle {
            font-family: PingFangSC-Regular,sans-serif;
            color: #000000;
            font-size: 1.5rem;
            margin-left: 20px;
            font-weight: 100;
        }

        .productCardIconSub{
            font-family: PingFangSC-Regular,sans-serif;
            color: #707070;
            font-size: 1rem;
            margin-left: 20px;
            font-weight: 100;
        }

        /*提示箭头的样式*/
        .P1Enter{
            display: flex;
            background-color:#CAEBFB;
            height: 198px;
            width: 80px;
            position: absolute;
            z-index: 100;
            top: 1100px;
            right: 0;
            align-items: center;
            justify-content: center;
        }

        .P1Enter img{
            display: inline-flex;
            height: 22px;
        }

        .P2Enter{
            display: flex;
            background-color:#F2F2FA;
            height: 198px;
            width: 80px;
            position: absolute;
            z-index: 100;
            top: 1300px;
            right: 0;
            align-items: center;
            justify-content: center;
        }

        .P2Enter img{
            display: inline-flex;
            height: 22px;
        }

        .P3Enter{
            font-family: PingFangSC-Regular,sans-serif;
            display: flex;
            background:linear-gradient(to right,rgba(255,216,105,0),rgba(255,175,56,0.5));
            color: #996921;
            height: 2rem;
            width: 180px;
            position: absolute;
            top: 1571px;
            right: 10%;
            align-items: center;
            justify-content: flex-end;
            padding-right: 15px;
            border-radius: 5px;

        }


        /*P1左三角形*/
        .triangle{
            display: flex;
            position: absolute;
            width: 0;
            height: 0;
            border-left: 20px solid transparent;
            border-right: 20px solid #FFFFFF;
            border-bottom: 20px solid transparent;
            border-top: 20px solid transparent;
            right: 34%;
            top: 1180px;
        }

        /*P2左三角形*/
        .P2triangle{
            display: flex;
            position: absolute;
            width: 0;
            height: 0;
            border-left: 20px solid transparent;
            border-right: 20px solid #FFFFFF;
            border-bottom: 20px solid transparent;
            border-top: 20px solid transparent;
            right: 34%;
            top: 1380px;
        }

        /*P3左三角形*/
        .P3triangle{
            display: flex;
            position: absolute;
            width: 0;
            height: 0;
            border-left: 20px solid transparent;
            border-right: 20px solid #FFFFFF;
            border-bottom: 20px solid transparent;
            border-top: 20px solid transparent;
            right: 34%;
            top: 1580px;
        }
        /*合作伙伴评价*/
        .impressionContainer {
            font-family: PingFangSC-Regular,sans-serif;
            display: flex;
            justify-content: center;
            min-width: 1270px;
            height: 450px;
        }


        .impression {
            display: flex;
            flex-direction: column;
            align-items: center;

        }

        .impression  h1{
            font-family: PingFangSC-Regular,sans-serif;
            color: #695229;
            margin: 50px;
            font-size: 1.4rem;
            font-weight: 500;
        }

        .impression .content {
            width: 600px;
            box-shadow: 0 0 30px rgba(20,89,193,0.2) ;

        }

        .impression p{
            font-family: PingFangSC-Regular,sans-serif;
            padding: 20px 100px;
            line-height: 2rem;
            color: #373150;
        }

        .customer{
            display: flex;
            margin-top: 30px;
        }

        .customer img{
            width: 70px;
        }

        .customer h1{
            font-family: PingFangSC-Regular,sans-serif;
            margin: 10px 0 0 10px;
            font-size: 1.2rem;
        }

        .customer p{
            font-family: PingFangSC-Regular,sans-serif;
            padding: 0;
            margin-left: 10px;
            font-size: 0.8rem;
        }

        .customer .info {
            display: flex;
            flex-direction: column;
        }

        /*酒店简介的样式*/

        .hotelContainer{
            display: flex;
            min-width: 1270px;
            background-color: #1175BC;
        }

        .hotelContainer .left{
            background-image: url("../assets/hotelLobby.jpg");
            background-repeat: no-repeat;
            background-size: 100%;
            height: 520px;
            width: 65%;
        }

        .hotelContainer .right{
            width: 35%;
            background-color: #1175BC;
        }

        .hotelContainer h1{
            font-family: PingFangSC-Regular,sans-serif;
            font-weight: 400;
            color: #FFFFFF;
            margin-top: 40px;
            font-size: 60px;
            padding: 20px 80px 20px 40px;
        }

        .hotelContainer p {
            font-family: PingFangSC-Regular,sans-serif;
            color: #FFFFFF;
            padding: 10px 40px 10px 40px;
        }

        .hotelContainer a{
            font-family: PingFangSC-Regular,sans-serif;
            display: inline-flex;
            background-color: #FFFFFF;
            text-decoration: none;
            padding: 10px 30px;
            margin: 20px 40px;
            color: black;
            font-size: 14px;
        }

        /*营销之路*/
        .marketingContainer{
            display: flex;
            flex-direction: column;
            align-items: center;
            min-width: 1270px;
        }

        .marketingContainer h1{
            font-family: PingFangSC-Regular,sans-serif;
            color: #695229;
            font-weight: 400;
            padding: 50px 50px 10px 50px;
        }

        .marketingContainer h2{
            font-family: PingFangSC-Regular,sans-serif;
            color: #707070;
            font-weight: 400;
            font-size: 18px;
        }

        .marketingContainer img{
            margin: 40px 40px 160px;
            width: 40%;
        }

        /*footer样式*/
        .footerContainer{
            display: flex;
            flex-direction: column;
            align-items: center;
            background-color: #454545;
            height: auto;
        }

        .contentContainer{
            display: flex;
            border-bottom: 1px solid #707070;
            width: 1270px;
            padding-bottom: 40px;
        }

        .footer {
            display: flex;
            justify-content: space-between;
            width: 100%;
        }

        .footerContainer h1{
            font-family: PingFangSC-Regular,sans-serif;
            color: #FFFFFF;
            font-size: 16px;
            margin: 60px 0 20px;
            font-weight: lighter;
        }

        .footerContainer ul {
            font-family: PingFangSC-Regular,sans-serif;
            padding-left: 0;
            list-style: none;
        }

        .footerContainer li{
            font-family: PingFangSC-Regular,sans-serif;
            color: #B1B1B1;
            padding-bottom: 10px;
        }

        .footerContainer span{
            font-family: PingFangSC-Regular,sans-serif;
            color: #E5C182;
        }

        .footerContainer a{
            font-family: PingFangSC-Regular,sans-serif;
            text-decoration: none;
            color: #B1B1B1;
        }

        .footerContainer p{
            font-family: PingFangSC-Regular,sans-serif;
            margin: 60px 0 80px;
            color: #B1B1B1;
            font-size: 14px;
        }



</style>
