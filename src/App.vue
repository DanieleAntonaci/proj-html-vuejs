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
  <div id="up-page">
    <a href="#">
      <font-awesome-icon icon="fa-solid fa-angle-up" />
    </a>
  </div>
</template>

<style lang="scss">
@use './style/general.scss' as *;
@use './style/partials/mixin' as *;
@use './style/partials/variables' as *;

#up-page {
  position: fixed;
  bottom: 5px;
  right: 30px;
  opacity: .7;

  a {
    color: white;
    background-color: gray;
    padding: 15px 15px 20px;
    border-radius: 7px 7px 0 0;
  }
}
</style>
