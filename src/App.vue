<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />

  </div>
</template>

<script>

import Header from './components/Header.vue';

import Main from './components/Main.vue';
import Footer from './components/Footer.vue';



export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer

  }
}
</script>

<style lang="scss">

@import '~bootstrap/scss/bootstrap.scss';
@import '~@fontsource/merriweather/index.css';
@import '~@fontsource/merriweather/700.css';
@import './assets/style/vars.scss';





</style>


