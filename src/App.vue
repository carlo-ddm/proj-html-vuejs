<template>
  <div id="app">
    <HeaderComp />
    <JumbotronComp />
    <MainComp />
    <FooterComp />
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import FooterComp from './components/FooterComp.vue';
import JumbotronComp from './components/JumbotronComp.vue';


export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp,
    JumbotronComp
}
}
</script>

<style lang="scss">
// Import Bootstrap
@import '~bootstrap/scss/bootstrap.scss';
// Import Fontsource
@import '~@fontsource/roboto/index.css';
// Import Fontawesome
@import '~@fortawesome/fontawesome-free/css/all.min.css'


</style>
