<template>
    <ul>
        <li>
            <a href="#">DC</a>
        </li>
        <li>
            <a href="#">Terms Of Use</a>
        </li>
        <li>
            <a href="#">Privacy policy (New)</a>
        </li>
        <li>
            <a href="#">Ad Choices</a>
        </li>
        <li>
            <a href="#">Advertising</a>
        </li>
        <li>
            <a href="#">Jobs</a>
        </li>
        <li>
            <a href="#">Subscriptions</a>
        </li>
        <li>
            <a href="#">Talent Workshops</a>
        </li>
        <li>
            <a href="#">CPSC Certificates</a>
        </li>
        <li>
            <a href="#">Ratings</a>
        </li>
        <li>
            <a href="#">Shop Help</a>
        </li>
        <li>
            <a href="#">Contact Us</a>
        </li>
    </ul>
</template>

<script>
    export default {
       name: "DCMenu", 
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