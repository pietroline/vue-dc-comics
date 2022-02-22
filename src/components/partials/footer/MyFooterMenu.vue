<template>

    <ul>
        <li>
            <a :href="titleList.src">{{titleList.text}}</a>
        </li>
        <li v-for="(item, index) in menuList" :key="index">
            <a :href="item.src">{{item.text}}</a>
        </li>
    </ul>

</template>

<script>
    export default {
        name: "MyFooterMenu",
        props: ["titleList", "menuList"],
    }
</script>

<style lang="scss" scoped>

    @import "./../../../assets/style/variables.scss";

    ul{

        list-style: none;
        padding: 0.5rem 1.5rem;

        li:first-child{
                text-transform: uppercase;
                font-weight: bold;
                font-size: 1.3rem;

                margin-bottom: 0.2rem;

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