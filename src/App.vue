<template>
  <div>

    <header>
      <div class="spazioCentro">
        <LogoDC/>
        <NavHeader/>
      </div>
    </header>

    <main>
        <MyMain/>
    </main>

    <footer>
      <div class="footerUp">
        <div class="container"><MyBlueBand/></div>
      </div>
      <div class="footerDown">
          <div class="container spazioCentro">
            <SingUpNow/>
            <FollowUs/>
          </div>
      </div>
    </footer>
  
  </div>
</template>

<script>
import LogoDC from './components/LogoDC.vue';
import NavHeader from './components/NavHeader.vue';
import MyMain from './components/MyMain.vue';
import MyBlueBand from './components/MyBlueBand.vue';
import SingUpNow from './components/SingUpNow.vue';
import FollowUs from './components/FollowUs.vue';


export default {
  name: 'App',
  components: {
    LogoDC,
    NavHeader,
    MyMain,
    MyBlueBand,
    SingUpNow,
    FollowUs,
  }
}
</script>

<style lang="scss">

  @import "./assets/style/general.scss";
  @import "./assets/style/variables.scss";

  .spazioCentro{
      display: flex;
      align-items: center;
      justify-content: space-between;
  }

  header{
       @include centroPagina;
  }

  main{
    background-color: $colorMain;
  }

  footer{

    .footerUp{
      background-color: $colorBlue;

      .container{
         @include centroPagina;
      }
    }

    .footerDown{
      background-color: $coloreNeroFooter;
      padding: 2rem 0;

      .container{
         @include centroPagina;
      }
    }

  }
</style>
