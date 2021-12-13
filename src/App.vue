<template>
  <div id="app">
    <Header />
    <Subject />
    <Main />
    <Footer />

  </div>
</template>

<script>

import Header from './components/Header.vue';
import Subject from './components/Subject.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';



export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    Subject

  }
}
</script>

<style lang="scss">

@import '~bootstrap/scss/bootstrap.scss';
@import '~@fontsource/merriweather/index.css';
@import '~@fontsource/merriweather/700.css';
@import './assets/style/vars.scss';





</style>


