<template>
  <div class="product">

    <div class="container product-list" >

        <div class="card" v-for="(link,index) in links" :key="index">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <!--<img :src="`../assets/img/${link.img}`" alt="">-->
          <a :href="link.url">{{link.text}}</a>
        </div>

        <!--<div class="card">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <a href="#">Digital Comics</a>
        </div>

        <div class="card">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <a href="#">Digital Comics</a>
        </div>

        <div class="card">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <a href="#">Digital Comics</a>
        </div>

        <div class="card">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <a href="#">Digital Comics</a>
        </div> -->

    </div>
 
  </div>
</template>

<script>
export default {
  name: 'MyProduct',
  data() {
    return {
      links: [
        {
          text: "Digital Comics",
          url: "#",
          img: "buy-comics-digital-comics.png"
        },
        {
          text: "dc merchandise",
          url: "#",
          img: "buy-comics-merchandise.png",
        },
        {
          text: "subscription",
          url: "#",
          img: "buy-comics-shop-locator.png",
        },
        {
          text: "comic shop locator",
          url: "#",
          img: "buy-comics-subscriptions.png",
        },
        {
          text: "dc power visa",
          url: "#",
          img: "buy-dc-power-visa.svg",
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/variables.scss";

.product{
  background-color: $secondaryColor;
  height: 200px;
}

img{
  width: 50px;
}

.product-list{
  display: flex;
  height: 100%;
  justify-content: space-around;
  align-items: center;

  .card{
    display: flex;
    align-items: center;

    a{
      margin-left: 10px;
      text-decoration: none;
      text-transform: uppercase;
      color: $tertiaryColor;
    }
  }

}
</style>
