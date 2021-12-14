<template>
  <section>
    <PatternSection />
  </section>

</template>

<script>

import PatternSection from './PatternSection.vue';

export default {
  name: 'PatternContainer',
  components:{ 
    PatternSection
  }
}
</script>

<style lang="scss">

@import '../assets/style/vars.scss';
@import '../assets/style/mixins.scss';

section{
  background-image: url(../assets/img/page-background-img.png);
  @include background-cover;
  background-size: 190%;
  background-position: 75% 0%;
}

</style>