<template>
  <div>

    <header>
      <LogoDC/>
      <NavHeader/>
    </header>

    <main>
        <MyMain/>
    </main>

    <footer>
      <MyBlueBand/>
    </footer>
  
  </div>
</template>

<script>
import LogoDC from './components/LogoDC.vue';
import NavHeader from './components/NavHeader.vue';
import MyMain from './components/MyMain.vue';
import MyBlueBand from './components/MyBlueBand.vue';

export default {
  name: 'App',
  components: {
    LogoDC,
    NavHeader,
    MyMain,
    MyBlueBand,
  }
}
</script>

<style lang="scss">

  @import "./assets/style/general.scss";
  @import "./assets/style/variables.scss";


  header{
    display: flex;
    align-items: center;
    justify-content: space-between;

    @include centroPagina;
  }

  main{
    background-color: $colorMain;
  }
</style>
