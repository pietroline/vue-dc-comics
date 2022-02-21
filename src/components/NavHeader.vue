<template>
    <nav>

        <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>Tv</li>
            <li>Games</li>
            <li>Collectibles</li>
            <li>Videos</li>
            <li>Fans</li>
            <li>News</li>
            <li>Shop</li>
        </ul>

    </nav>
</template>

<script>
    export default {
        name:"NavHeader"
    }
</script>

<style scoped lang="scss">

    nav{
        text-transform: uppercase;

        li{
            display: inline-block;

            padding: 1rem;

            font-weight: bold;
            font-size: 0.8rem;
        }
    }

</style>
