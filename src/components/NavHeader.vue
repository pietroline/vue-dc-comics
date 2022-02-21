<template>
    <nav>

        <ul>
            <li>
                <a href="#">Characters</a>
            </li>
            <li class="active">
                <a href="#">Comics</a>
            </li>
            <li>
                <a href="#">Movies</a>
            </li>
            <li>
                <a href="#">Tv</a>
            </li>
            <li>
                <a href="#">Games</a>
            </li>
            <li>
                <a href="#">Collectibles</a>
            </li>
            <li>
                <a href="#">Videos</a>
            </li>
            <li>
                <a href="#">Fans</a>
            </li>
            <li>
                <a href="#">News</a>
            </li>
            <li>
                <a href="#">Shop</a>
            </li>
        </ul>

    </nav>
</template>

<script>
    export default {
        name:"NavHeader"
    }
</script>

<style scoped lang="scss">

    @import "./../assets/style/variables.scss";

    nav{
        text-transform: uppercase;

        li{
            display: inline-block;

            padding: 1rem;

            font-weight: bold;
            font-size: 1rem;

            a{
                text-decoration: none;
                color: $coloreNero; 
            }

            &:hover a{
                color: $colorBlue;
                border-bottom: 5px solid $colorBlue;
                padding: 4rem 0;
            }  
        }

        .active{
            border-bottom: 5px solid $colorBlue;
            padding: 4rem 0;

            a{
                color: $colorBlue;
            }
        }
    }

</style>
