<template>
  <main>
    <Subject />
    <SectionRow />
    <SectionColumn />
  </main>
</template>

<script>

import Subject from './Subject.vue';
import SectionRow from './SectionRow.vue';
import SectionColumn from './SectionColumn.vue';


export default {
  name: 'Main',
  components:{ 
    Subject,
    SectionRow,
    SectionColumn,
  }
}
</script>

<style lang="scss">
//IMPORT STYLE
@import '../assets/style/vars.scss';

</style>