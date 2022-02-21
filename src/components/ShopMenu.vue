<template>
    <ul>
        <li>
            <a href="#">SHOP</a>
        </li>
        <li>
            <a href="#">Shop DC</a>
        </li>
        <li>
            <a href="#">Shop DC Collectibles</a>
        </li>
       
    </ul>
</template>

<script>
    export default {
       name: "DCComicsMenu", 
    }
</script>

<style lang="scss" scoped>

    @import "./../assets/style/variables.scss";

    ul{

        list-style: none;
        padding: 2rem 3rem;

        li:first-child{
                text-transform: uppercase;
                font-weight: bold;

                margin-bottom: 1rem;

                a{
                    color: #fff;
                }
            }

        a{
            text-decoration: none;
            color: $coloreTestoGrigio;
        }

        li{
            padding: 0.2rem 0;
        }
    }
</style>