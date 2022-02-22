<template>

   <div  class="card">

       <div class="contenitoreImg">

            <a href="#">
                <img :src="item.thumb" :alt="'img DC type ' + item.type">
            </a>
            <div class="price">{{item.price}}</div>

       </div>
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

        &:hover h5{
            color: #fff;
        }

        .contenitoreImg{
            position: relative;
        }

        .price{
            color: #fff;
            font-weight: bold;
            font-size: 2rem;

            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);

            display: none;
        }
        
        &:hover .price{
            display: block;
        }

        &:hover img{
            opacity: 0.3;
        }

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