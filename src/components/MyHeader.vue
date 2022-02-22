<template>
  <nav class="container">
    <!--nav sx-->
    <div class="nav-left">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>

    <!--nav dx-->
    <div class="nav-right">
      <ul>
        <!--Popolamento dinamico delle voci del menu-->
        <li v-for="(link,index) in links" :key="index" >
          <a :href="link.url"  @click="menuActive(index)" :class="(index == active) ? 'active':''">{{link.text}}</a>
        </li>
      </ul>
    </div>

  </nav>
    

  
</template>

<script>
export default {
  name: 'MyHeader',
  //cambio dinamico della voce del menu con la classe active al click
  methods: {
      menuActive(index){
        this.active = index;
      }
  },
  data() {
    return {
      active: 1,
      links: [
          {
              text: "Characters",
              url: "#"
          },
          {
              text: "Comics",
              url: "#"
          },
          {
              text: "Movies",
              url: "#"
          },
          {
              text: "Tv",
              url: "#"
          },
           {
              text: "Games",
              url: "#"
          },
          {
              text: "Collectibles",
              url: "#"
          },
           {
              text: "Videos",
              url: "#"
          },
          {
              text: "Fans",
              url: "#"
          },
           {
              text: "News",
              url: "#"
          },
          {
              text: "Shop",
              url: "#"
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
    padding:0 6px 61px 6px ;

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
