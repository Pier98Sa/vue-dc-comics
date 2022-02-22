<template>
  
    <div class="product-card" >
        <div class="photo-card">
            <img :src="src" :alt="title">
        </div>

        <p>{{title}}</p>

    </div>

</template>

<script>
export default {
    name: "ProductCard",
    props: {
        title: String,
        src: String
    }

}
</script>

<style scoped lang="scss">
    
    .product-card{
      width: calc(100% / 6);
      padding: 20px;

      .photo-card{
        width: 185px;
        height: 185px;
        overflow: hidden;

      }

      p{
        padding-top: 10px;
      }
    }
        
</style>