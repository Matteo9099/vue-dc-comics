<template>
  <div id="app">
    
    <HeaderComponents />
    <JumbotronComponents />
    <MainComponents />
    <MainNavMenu />
    <FooterComponents />

  </div>
</template>

<script>
import HeaderComponents from './components/HeaderComponents.vue'
import MainComponents from './components/MainComponents.vue'
import FooterComponents from './components/FooterComponents.vue'
import JumbotronComponents from './components/JumbotronComponents.vue'
import MainNavMenu from './components/MainNavMenu.vue'

export default {
  name: 'App',
  components: {
    HeaderComponents,
    MainComponents,
    FooterComponents,
    JumbotronComponents,
    MainNavMenu
  }
}
</script>

<style lang="scss">

    @import "assets/style/general.scss";


</style>
