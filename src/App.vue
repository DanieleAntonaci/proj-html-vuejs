<script>
import Footer from './components/Footer.vue';
import Header from './components/Header.vue'
import Main from './components/Main.vue';
export default {
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<template>
  <Header/>
  
  <Main/>

  <Footer/>
</template>

<style lang="scss">
@use './style/general.scss' as *;
@use './style/partials/mixin' as *;
@use './style/partials/variables' as *;
</style>
