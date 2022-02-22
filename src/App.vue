<template>
  <div>

    <header>
      <MyHeader/>
    </header>

    <main>
        <MyMain/>
    </main>

    <footer>
      <MyFooter/>
    </footer>
  
  </div>
</template>

<script>

  import MyHeader from "./components/MyHeader.vue"
  import MyMain from './components/MyMain.vue';
  import MyFooter from './components/MyFooter.vue';

  export default {
    name: 'App',
    components: {
      MyHeader,
      MyMain,
      MyFooter,
    }
  } 
  
</script>

<style lang="scss">

  @import "./assets/style/general.scss";
  @import "./assets/style/variables.scss";

  header{
       @include centroPagina;
  }

  main{
    background-color: $colorMain;
  }

</style>
