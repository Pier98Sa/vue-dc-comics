<template>
  <div id="app">
    <MyHeader/>
    <MyJumbotron/>
    <MyMain/>
    <MyProduct/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyJumbotron from './components/MyJumbotron.vue'
import MyProduct from './components/MyProduct.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbotron,
    MyMain,
    MyProduct,
    MyFooter
  }
}
</script>

<style lang="scss">
@import "./assets/style/general.scss";
</style>
