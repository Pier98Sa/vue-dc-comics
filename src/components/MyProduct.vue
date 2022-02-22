<template>
  <div class="product">

    <div class="container product-list" >

      <div class="card" v-for="(link,index) in links" :key="index">
        <img :src="link.img" alt="">
        <a :href="link.url">{{link.text}}</a>
      </div>

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
          img: require("../assets/img/buy-comics-digital-comics.png")
        },
        {
          text: "dc merchandise",
          url: "#",
          img: require("../assets/img/buy-comics-merchandise.png")
        },
        {
          text: "subscription",
          url: "#",
          img: require("../assets/img/buy-comics-subscriptions.png")
        },
        {
          text: "comic shop locator",
          url: "#",
          img: require("../assets/img/buy-comics-shop-locator.png")
        },
        {
          text: "dc power visa",
          url: "#",
          img: require("../assets/img/buy-dc-power-visa.svg")
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
  height: 50px;
  object-fit: contain;
  
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
      font-size: 13px;
      color: $tertiaryColor;
    }
  }

}
</style>
