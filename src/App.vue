<template>
  <div>

    <header>
      <LogoDC/>
      <NavHeader/>
  </header>

  <main>

  </main>
  
  </div>
</template>

<script>
import LogoDC from './components/LogoDC.vue';
import NavHeader from './components/NavHeader.vue';

export default {
  name: 'App',
  components: {
    LogoDC,
    NavHeader,
  }
}
</script>

<style lang="scss">

  @import "./assets/style/general.scss";

  header{
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
</style>
