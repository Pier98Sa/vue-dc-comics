<template>
  <footer>
    <div class="footer-top container">
      <div class="footer-menu">
        <div class="col sx">
          <h2>Dc Comics</h2>
        <ul>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
        </ul>

        <h2>Shop</h2>
        <ul>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>
        </div>
        <div class="col center">
          <h2>DC</h2>
        <ul>
          <li><a href="#">Terms of Use</a></li>
          <li><a href="#">Privacy policy (New)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshop</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact US</a></li>
        </ul>
        </div>

        <div class="col dx">
          <h2>Sites</h2>
          <ul>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>
        </div>
        

        
      </div>

      <div class="logo">
        <img src="../assets/img/dc-logo-bg.png" alt="dc logo">
      </div>

    </div>

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
export default {
  name: 'MyFooter',
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
      display: flex;
      

      .col{
        padding: 20px;    

        h2{
          color: $tertiaryColor;
          font-size: 20px;
          text-transform: uppercase;
          padding: 10px 0 10px 0;
        }

        li{
          list-style: none;

          a{
            text-decoration: none;
            color: $quaternaryColor;
            font-size: 12px;
            padding: 10px 0 10px 0;
          }
        }

      }
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
