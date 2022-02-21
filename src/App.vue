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

      <div class="footerMiddle">
        <div class="container">

          <div class="flex">

            <div class="flex-column">
              <DCComicsMenu/>
              <ShopMenu/>
            </div>

            <DCMenu/>
            <SitesMenu/>
            <img src="./assets/img/dc-logo-bg.png" alt="">

          </div>

        </div>
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
import DCComicsMenu from './components/DCComicsMenu.vue';
import DCMenu from './components/DCMenu.vue';
import SitesMenu from './components/SitesMenu.vue';
import ShopMenu from './components/ShopMenu.vue';
import SingUpNow from './components/SingUpNow.vue';
import FollowUs from './components/FollowUs.vue';

export default {
  name: 'App',
  components: {
    LogoDC,
    NavHeader,
    MyMain,
    MyBlueBand,
    DCComicsMenu,
    DCMenu,
    SitesMenu,
    ShopMenu,
    SingUpNow,
    FollowUs,
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

  footer{

    .footerUp{
      background-color: $colorBlue;

      .container{
         @include centroPagina;
      }
    }

    .footerMiddle{
      background-image: url("./assets/img/footer-bg.jpg");
      background-size: cover;

        .container{
          @include centroPagina;
          
          padding: 3rem 0;
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
