<template>
  <section class="pattern-container">
    <PatternSection />
    <PlansSection />
  </section>

</template>

<script>

import PatternSection from './PatternSection.vue';
import PlansSection from './PlansSection.vue';

export default {
  name: 'PatternContainer',
  components:{ 
    PatternSection,
    PlansSection
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