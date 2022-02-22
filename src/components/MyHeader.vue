<template>
  <div class="spazioCentro">
        <LogoDC/>
        <NavHeader/>
  </div>
</template>

<script>

    import LogoDC from "./partials/header/LogoDC.vue";
    import NavHeader from "./partials/header/NavHeader.vue";

    export default {
        name: "MyHeader",
        components:{
            LogoDC,
            NavHeader,
        }
    }
</script>

<style>


</style>