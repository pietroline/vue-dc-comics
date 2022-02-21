<template>
    <ul>
        <li>
            <a href="#">DC</a>
        </li>
        <li>
            <a href="#">MAD Magazine</a>
        </li>
        <li>
            <a href="#">DC Kinds</a>
        </li>
        <li>
            <a href="#">DC Universe</a>
        </li>
        <li>
            <a href="#">DC Power Visa</a>
        </li>
    </ul>
</template>

<script>
    export default {
       name: "SitesMenu", 
    }
</script>

<style lang="scss" scoped>

    @import "./../assets/style/variables.scss";

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