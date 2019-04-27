<template>
<div id="container" >
    <div id="banner" class="bannerImg">
        <h1>微信生态+PC网页端</h1>
        <h1>一体化酒店智慧营销管理解决方案</h1>
        <h2>助力粉丝留存，增加酒店收入</h2>
        <a href="#">免费试用30天</a>
    </div>
    <header></header>
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

        }

        .bannerImg a{
            
        }


</style>
