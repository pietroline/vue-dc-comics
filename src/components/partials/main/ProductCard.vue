<template>

   <div  class="card">
        <img :src="item.thumb" alt="">
        <h5>{{item.series}}</h5>
    </div>

</template>

<script>
    export default {
        name: "ProductCard",
        props:["item"]
    }
</script>

<style lang="scss" scope>

    @import "./../../../assets/style/variables.scss";

    .card{
        width: calc(100% / 6);
        padding: 1.5rem 0.8rem;

        img{
            width: 100%;
            height: 10rem;
            object-fit: cover;
            object-position: top;
        }

        h5{
            text-transform: uppercase;
            color: $coloreTestoGrigio;

            margin: 0.3rem 0;
        }
    }

</style>