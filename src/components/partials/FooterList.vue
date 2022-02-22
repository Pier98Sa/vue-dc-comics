<template>
  <div class="col">

      <h2>{{title}}</h2>
      
        <ul>
            <li v-for="(item, index) in items" :key="index">
                <a :href="item.src">{{item.text}}</a>
            </li>
        </ul>
     
  </div>
</template>

<script>
export default {
    name: "FooterList",
    props: {
        title: String,
        items: Array
    }

}
</script>

<style scoped lang="scss">
    @import "../../assets/style/variables.scss";
    
        .col{
            padding: 10px;
            
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
</style>