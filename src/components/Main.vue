<template>
  <main>
    <Subject />
    <Section />
  </main>
</template>

<script>

import Subject from './Subject.vue';
import Section from './Section.vue';


export default {
  name: 'Main',
  components:{ 
    Subject,
    Section
  }
}
</script>

<style lang="scss">
//IMPORT STYLE
@import '../assets/style/vars.scss';

</style>