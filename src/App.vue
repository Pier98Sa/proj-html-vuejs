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
  @import './style/variables.scss';
  #app{
    font-family: Arial, Helvetica, sans-serif;
  }

  .my_container{
    max-width: 980px;
    width: 100%;
    margin: 0 auto;
  }
  .ms_btn-green{
    background-color: $quinaryColorHeader;
    border-radius: 16px;
    border: none;
    font-size: 12px;
    text-transform: uppercase;
    padding: 8px 16px;

    &:hover{
      background-color: $senaryColorHeader;
    }
  }
</style>
 