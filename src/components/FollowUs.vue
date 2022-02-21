<template>
    <div class="contenitore">

        <span>FOLLOW US</span>
        
        <a href="#">
            <img src="./../assets/img/footer-facebook.png" alt="Img logo Facebook">
        </a>

        <a href="#">
            <img src="./../assets/img/footer-twitter.png" alt="Img logo Twitter">
        </a>

        <a href="#">
            <img src="./../assets/img/footer-youtube.png" alt="Img logo Youtube">
        </a>

        <a href="#">
            <img src="./../assets/img/footer-pinterest.png" alt="Img logo Pinterest">
        </a>

        <a href="#">
            <img src="./../assets/img/footer-periscope.png" alt="Img logo Periscope">
        </a>   

    </div>
</template>

<script>
    export default {
        name: "FollowUs",
    }
</script>

<style lang="scss" scoped>

     @import "./../assets/style/variables.scss";

    .contenitore{
        color: $colorBlue;
        font-weight: bold;

        display: flex;
        align-items: center;

        span{
            margin-right: 1rem;
        }

        a{
            margin: 0 0.8rem;
        }
    }

</style>