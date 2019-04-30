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
            <img src="../assets/wechatDash.png" alt="wechatDash" width="600">
        </div>
        <div class="right"></div>
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
    <footer class="footerContainer"></footer>
</div>
</template>

<script>
    export default {
        name: "home"
    }
</script>

<style scoped>
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
            color: #FFFFFF;
            font-size: 2rem;
            font-weight: 400;
        }

        .bannerImg h2{
            color: #FFFFFF;
            margin-top: 10px;
            font-size: 1.2rem;
            font-weight: 400;
        }

        .bannerImg a{
            width: 160px;
            height: 50px;
            text-align: center;
            line-height: 50px;
            font-size: 0.9rem;
            text-decoration: none;
            color: #695229;
            font-weight: 700 ;
            background-color: #FFFFFF;
            border-radius: 50px;
            margin-top: 30px;

        }

        .headerContainer {
            display: flex;
            width: 100%;
            height: 80px;
            /*background-color: blue;*/
            position: absolute;
            align-items: center;
            justify-content: center;
            min-width: 1270px;
        }

        .header{
            display: flex;
            width: 1270px;
            /*background-color: red;*/
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
            /*line-height: 40px;*/
        }

        .header ul li a{
            text-decoration: none;
            list-style: none;
            float: left;
            color: #FFFFFF

        }

        li + li{
            margin-left: 10px;
        }

        .header ul li a:hover{
            border-bottom: 2px solid #FFFFFF  ;
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
            color: #707070;
            font-size: 1rem;
            margin: 10px ;
        }

        .dashboard .item h2{
            color: #707070;
            font-size: 0.8rem;
            margin: 0 0 40px ;
            font-weight: 300;
        }

        .dashboard .item  img{
            width: 40px;
        }

        .productContainer{
            display: flex;
            min-width: 1270px;
        }

        .productContainer .left{
            display: flex;
            width: 66%;
            height: 400px;
            background: linear-gradient(#CCEDFC, #9FD1F5);
            justify-content: center;
            align-items: center;
        }

        .productContainer .right{
            width: 34%;
            height: 400px;
            background-color: #FFFFFF;
        }

        /*合作伙伴评价*/
        .impressionContainer {
            display: flex;
            justify-content: center;
            /*align-items: center;*/
            min-width: 1270px;
            height: 450px;
        }

        .impression {
            display: flex;
            flex-direction: column;
            align-items: center;

        }

        .impression  h1{
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
            margin: 10px 0 0 10px;
            font-size: 1.2rem;
        }

        .customer p{
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
            font-weight: 400;
            color: #FFFFFF;
            margin-top: 40px;
            font-size: 60px;
            padding: 20px 80px 20px 40px;
        }

        .hotelContainer p {
            color: #FFFFFF;
            padding: 10px 40px 10px 40px;
        }

        .hotelContainer a{
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
            color: #695229;
            font-weight: 400;
            padding: 50px 50px 10px 50px;
        }

        .marketingContainer h2{
            color: #707070;
            font-weight: 400;
            font-size: 18px;
        }

        .marketingContainer img{
            margin: 40px 40px 80px;
            width: 40%;
        }

        /*footer样式*/
        .footerContainer{
            background-color: #454545;
            height: 500px;
        }
</style>
