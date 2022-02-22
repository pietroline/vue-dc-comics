<template>
    <div class="fasciaBlu">
        <a href="#">
            <img src="./../../../assets/img/buy-comics-digital-comics.png" alt="Img comics digital">
            <h5>Digital Comics</h5>
        </a>
       

        <a href="#">
            <img src="./../../../assets/img/buy-comics-merchandise.png" alt="Img comics merchandaise">
            <h5>Dc merchandise</h5>
        </a>

        <a href="#">
            <img src="./../../../assets/img/buy-comics-subscriptions.png" alt="Img comics subscriptions">
            <h5>Subscription</h5>
        </a>

        <a href="#">
            <img class="locator" src="./../../../assets/img/buy-comics-shop-locator.png" alt="Img comics shop locator">
            <h5>comics shop locator</h5>
        </a>

        <a href="#">
            <img src="./../../../assets/img/buy-dc-power-visa.svg" alt="Img comics power visa">
            <h5>Dc power visa</h5>
        </a>
    </div>
</template>

<script>
    export default {
        name: "MyBlueBand",
    }
</script>

<style lang="scss" scoped>

    @import "./../../../assets/style/variables.scss";

    .fasciaBlu{

        width: 70%;
        margin: 0 auto;

        background-color: $colorBlue;

        height: 8rem;
        width: 100%;

        display: flex;
        align-items: center;
        justify-content: center;

        a{
            text-decoration: none;
            text-transform: uppercase;
            color: #fff;
            
            display: flex;
            align-items: center;

            padding: 0 2rem;

            img{
               height: 3rem;
            }

            h5{
                padding-left: 1rem;
                font-size: 0.9rem;
            }
        }
    }

</style>