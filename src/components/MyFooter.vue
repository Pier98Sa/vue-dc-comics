<template>
  <footer>
    <!--footer top-->
    <div class="footer-top container">
      <div class="footer-menu">
        <!--footer menu popolato dinamicamente con componente esterno-->
        <FooterList :title="'Dc Comics'" :items="dcComics"></FooterList>
        <FooterList :title="'Shop'" :items="shop"></FooterList>
        <FooterList :title="'Dc'" :items="dc"></FooterList>
        <FooterList :title="'Sites'" :items="sites"></FooterList>
      </div>

      <div class="logo">
        <img src="../assets/img/dc-logo-bg.png" alt="dc logo">
      </div>

    </div>

    <!--Footer bottom-->
    <div class="footer-bottom ">
      <div class="container footer-bottom-items">

        <div class="left">
          <button> <a href="#">Sign-up now!</a> </button>
        </div>

        <div class="right">
          <span>Follow us</span>
          <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
          <a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
          <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
          <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
          <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope"></a>

        </div>
      </div>
      

    </div>

  </footer>
</template>

<script>

import FooterList from './partials/FooterList.vue';
export default {
  name: 'MyFooter',
  components:{
    FooterList
  },
  data(){
    return{
      dcComics:[
        {
          src: "#",
          text: "Characters"
        },
        {
          src: "#",
          text: "Comics"
        },
        {
          src: "#",
          text: "Movies"
        },
        {
          src: "#",
          text: "TV"
        },
        {
          src: "#",
          text: "Games"
        },
        {
          src: "#",
          text: "Videos"
        },
        {
          src: "#",
          text: "News"
        }
        
      ],

      shop:[
        {
          src: "#",
          text: "Shop DC"
        },
        {
          src: "#",
          text: "Shop DC Collectibles"
        }  
      ],

      dc:[
        {
          src: "#",
          text: "Terms of Use"
        },
        {
          src: "#",
          text: "Privacy policy (New)"
        },
        {
          src: "#",
          text: "Ad Choices"
        },
        {
          src: "#",
          text: "Advertising"
        },
        {
          src: "#",
          text: "Jobs"
        },
        {
          src: "#",
          text: "Subscriptions"
        },
        {
          src: "#",
          text: "Talent Workshop"
        },
        {
          src: "#",
          text: "CPSC Certificates"
        },
        {
          src: "#",
          text: "Ratings"
        },
        {
          src: "#",
          text: "Shop Help"
        },
        {
          src: "#",
          text: "Contact US"
        }
        
      ],

      sites:[
        {
          src: "#",
          text: "DC"
        },
        {
          src: "#",
          text: "MAD Magazine"
        },
        {
          src: "#",
          text: "DC Kids"
        },
        {
          src: "#",
          text: "DC Universe"
        },
        {
          src: "#",
          text: "DC Power Visa"
        }
        
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/variables.scss";

footer{
  background-image: url(../assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 500px;

  .footer-top{
    height: 350px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    overflow: hidden;

    .footer-menu{
      height: 100%;
      display: flex; 
      flex-direction: column;
      flex-wrap: wrap;

    }

  }

  .footer-bottom{
    height: 150px;
    background-color: $primaryColor;

    .footer-bottom-items{
      display: flex;
      height: 100%;
      justify-content: space-between;
      align-items: center;

      .left button {
        background: none;
        border: solid 2px $secondaryColor;
        padding: 10px;

        a{
          text-decoration: none;
          text-transform: uppercase;
          font-size: 14px;
          color: $tertiaryColor;
        }
      }

      .right{
        display: flex;
        align-items: center;

        span{
          text-transform: uppercase;
          color: $secondaryColor;
          padding-right: 10px;
          font-weight: bold;
        }

        a{
          padding: 8px;
        }
      }
    }
  }
}


</style>
