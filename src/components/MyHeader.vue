<template>
  <nav class="container">
    <div class="Footer-left">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>

    <div class="Footer-right">
      <ul>
        <li v-for="(link,index) in links" :key="index">
          <a :href="link.url" :class="(link.current)? 'active' : '' ">{{link.text}}</a>
        </li>
        <!--
        <li><a href="#" class="active">Comics</a></li>
        <li><a href="#">Movies</a></li>
        <li><a href="#">Tv</a></li>
        <li><a href="#">Games</a></li>
        <li><a href="#">Collectibles</a></li>
        <li><a href="#">Videos</a></li>
        <li><a href="#">Fans</a></li>
        <li><a href="#">News</a></li>
        <li><a href="#">Shop</a></li>
        -->
      </ul>
    </div>

  </nav>
    

  
</template>

<script>
export default {
  name: 'MyHeader',
  data() {
    return {
      links: [
          {
              text: "Characters",
              url: "#",
              current: false,
          },
          {
              text: "Comics",
              url: "#",
              current: true,
          },
          {
              text: "Movies",
              url: "#",
              current: false,
          },
          {
              text: "Tv",
              url: "#",
              current: false,
          },
           {
              text: "Games",
              url: "#",
              current: false,
          },
          {
              text: "Collectibles",
              url: "#",
              current: false,
          },
           {
              text: "Videos",
              url: "#",
              current: false,
          },
          {
              text: "Fans",
              url: "#",
              current: false,
          },
           {
              text: "News",
              url: "#",
              current: false,
          },
          {
              text: "Shop",
              url: "#",
              current: false,
          }
      ],
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/variables.scss";

nav{
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 150px;
}

img{
  padding: 10px;
}

li{
  display: inline;
  padding: 10px;
  
  a{
    padding-bottom:61px ;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 12px;
    font-weight: bold;
    color: $primaryColor;
    

    &.active,
    &:hover{
      color: $secondaryColor;
      border-bottom: 4px solid $secondaryColor;
    }
  
  }
}
</style>
