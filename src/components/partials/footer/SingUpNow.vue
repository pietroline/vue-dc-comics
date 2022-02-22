<template>
    <div class="btn">SING-UP NOW!</div>
</template>

<script>
    export default {
        name: "SingUpNow",
    }
</script>

<style lang="scss" scoped>

    @import "./../../../assets/style/variables.scss";

    .btn{
        border: 2px solid $colorBlue;

        padding: 0.8rem;

        color: #fff;

        &:hover{
            cursor: pointer;
        }
    }

</style>