<template>
  <div id="app">
    <Header />
    <Jumbotron />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbotron from './components/Jumbotron.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import 'animate.css';
@import "~bootstrap";
@import "~@fortawesome/fontawesome-free/css/all.min.css";
@import "./assets/scss/style.scss";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  background-color: white;
}

body{
  min-width: 1834px;
  background-color: $color-brand;
}
</style>
