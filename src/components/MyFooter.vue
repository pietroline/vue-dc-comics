<template>
    <div>

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
            <img src="./../assets/img/dc-logo-bg.png" alt="">

          </div>

        </div>
      </div>

      <div class="footerDown">
          <div class="container spazioCentro">
            <SingUpNow/>
            <FollowUs/>
          </div>
      </div>

    </div>
</template>

<script>

    import DCComicsMenu from "./partials/footer/DCComicsMenu.vue";
    import DCMenu from "./partials/footer/DCMenu.vue";
    import FollowUs from "./partials/footer/FollowUs.vue";
    import MyBlueBand from "./partials/footer/MyBlueBand.vue";
    import ShopMenu from "./partials/footer/ShopMenu.vue";
    import SingUpNow from "./partials/footer/SingUpNow.vue";
    import SitesMenu from "./partials/footer/SitesMenu.vue";

    export default {
        name: "MyFooter",
        components: {
            DCComicsMenu,
            DCMenu,
            FollowUs,
            MyBlueBand,
            ShopMenu,
            SingUpNow,
            SitesMenu,
        }
    }
</script>

<style lang="scss" scoped>

    @import "./../assets/style/variables.scss";

    .footerUp{
        background-color: $colorBlue;

        .container{
            @include centroPagina;
        }
        }

    .footerMiddle{
      background-image: url("./../assets/img/footer-bg.jpg");
      background-size: cover;

      height: 30rem;
      overflow: hidden;

        .container{
          @include centroPagina;

          padding: 3rem 0;
          position: relative;

          img{
            height: 45rem;
            
            position: absolute;
            top: -8rem;
            right: 0;
          }
        }
    }

    .footerDown{
      background-color: $coloreNero;
      padding: 2rem 0;

      .container{
         @include centroPagina;
      }
    }
</style>