<template>
  <main>
    <Subject />
    <SectionRow />
    <SectionColumn />
    <ColorSection />
    <PossibilitiesSection />
    
  </main>
</template>

<script>

import Subject from './Subject.vue';
import SectionRow from './SectionColumn.vue';
import SectionColumn from './SectionRow.vue';
import ColorSection from './ColorSection.vue';
import PossibilitiesSection from './PossibilitiesSection.vue';


export default {
  name: 'Main',
  components:{ 
    Subject,
    SectionColumn,
    SectionRow,
    ColorSection,
    PossibilitiesSection,
  }
}
</script>

<style lang="scss">
//IMPORT STYLE
@import '../assets/style/vars.scss';

</style>