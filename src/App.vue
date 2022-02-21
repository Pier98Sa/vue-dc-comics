<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyProduct/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyProduct from './components/MyProduct.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyProduct,
    MyFooter
  }
}
</script>

<style lang="scss">
@import "./assets/style/general.scss";
</style>
