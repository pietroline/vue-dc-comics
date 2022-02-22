<template>
    <ul>
        <li>
            <a href="#">DC comics</a>
        </li>
        <li>
            <a href="#">Characters</a>
        </li>
        <li>
            <a href="#">Comics</a>
        </li>
        <li>
            <a href="#">Movies</a>
        </li>
        <li>
            <a href="#">TV</a>
        </li>
        <li>
            <a href="#">Games</a>
        </li>
        <li>
            <a href="#">Videos</a>
        </li>
        <li>
            <a href="#">News</a>
        </li>
    </ul>
</template>

<script>
    export default {
       name: "DCComicsMenu", 
    }
</script>

<style lang="scss" scoped>

    @import "./../../../assets/style/variables.scss";

    ul{

        list-style: none;
        padding: 0 1.5rem;

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

            &:hover{
                color: #fff;
            }
        }

        li{
            padding: 0.2rem 0;
        }
    }
</style>