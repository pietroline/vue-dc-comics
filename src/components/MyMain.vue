<template>
    <div class="container">
        <h1> --&gt; Content goes here &lt;-- </h1>
    </div>
</template>

<script>
    export default {
        name: "MyMain",
    }
</script>

<style lang="scss" scoped>

    @import "./../assets/style/variables.scss";

    .container{
        color: #fff;

        @include centroPagina;

        // provvisorio
        height: 8rem; 
        display: flex;
        align-items: center;
    }

</style>