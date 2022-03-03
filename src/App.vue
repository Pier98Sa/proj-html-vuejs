<template>
  <div id="app">
    <MyHeader/>
    <MyHero/>
    <MyMain/>
    <MyFooter/>
    
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyHero from './components/MyHero.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyHero,
    MyMain,
    MyFooter
  }
}
</script>

<style lang="scss">
  @import './style/general.scss';
  @import '~@fortawesome/fontawesome-free/css/all.css';

</style>
