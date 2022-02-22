<template>
    <div>

      <div class="footerUp">
        <div class="container"><MyBlueBand/></div>
      </div>

      <div class="footerMiddle">
        <div class="container">

          <div class="flex">

            <div class="flex-column">
              <MyFooterMenu :titleList="mainTitleDCComics" :menuList="menuDCComics"/>
              <MyFooterMenu :titleList="mainTitleShop" :menuList="menuShop"/>
            </div>

            <MyFooterMenu :titleList="mainTitleDC" :menuList="menuDC"/>
            <MyFooterMenu :titleList="mainTitleSites" :menuList="menuSites"/>
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

  import MyFooterMenu from "./partials/footer/MyFooterMenu.vue";
  
  
  import FollowUs from "./partials/footer/FollowUs.vue";
  import MyBlueBand from "./partials/footer/MyBlueBand.vue";
  import SingUpNow from "./partials/footer/SingUpNow.vue";

  export default {
      name: "MyFooter",
      components: {
          
        MyFooterMenu,

        FollowUs,
        MyBlueBand,
        SingUpNow,
      },
      data(){
        return{
          mainTitleDCComics: {
              src: "#",
              text: "DC comics",
            },
          mainTitleShop: {
              src: "#",
              text: "Shop",
            },
          mainTitleDC: {
              src: "#",
              text: "DC",
            },
          mainTitleSites: {
              src: "#",
              text: "Sites",
            },
      
          menuDCComics: [
            {
              src: "#",
              text: "Characters",
            },
            {
              src: "#",
              text: "Comics",
            },
            {
              src: "#",
              text: "Movies",
            },
            {
              src: "#",
              text: "TV",
            },
            {
              src: "#",
              text: "Games",
            },
            {
              src: "#",
              text: "Videos",
            },
            {
              src: "#",
              text: "News",
            },
          ],
          menuShop: [
            {
              src: "#",
              text: "Shop DC",
            },
            {
              src: "#",
              text: "Shop DC Collectibles",
            },
          ],
          menuDC: [
            {
              src: "#",
              text: "Terms Of Use",
            },
            {
              src: "#",
              text: "Privacy policy (New)",
            },
            {
              src: "#",
              text: "Ad Choices",
            },
            {
              src: "#",
              text: "Advertising",
            },
            {
              src: "#",
              text: "Jobs",
            },
            {
              src: "#",
              text: "Subscriptions",
            },
            {
              src: "#",
              text: "Talent Workshops",
            },
            {
              src: "#",
              text: "CPSC Certificates",
            },
            {
              src: "#",
              text: "Ratings",
            },
            {
              src: "#",
              text: "Shop Help",
            },
            {
              src: "#",
              text: "Contact Us",
            },
          ],
          menuSites: [
            {
              src: "#",
              text: "DC",
            },
            {
              src: "#",
              text: "MAD Magazine",
            },
            {
              src: "#",
              text: "DC Kinds",
            },
            {
              src: "#",
              text: "DC Universe",
            },
            {
              src: "#",
              text: "DC Power Visa",
            },
          ],
        }
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