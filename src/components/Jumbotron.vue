<template>
  <div class="jumbotron">
    
    <h1>
      Contemporary Ideas
    </h1>
    <div class="subtitle">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus distinctio reiciendis et laudantium odit aperiam ut impedit maxime optio sed dolorem, accusantium saepe.
    </div>
  </div>
</template>

<script>
export default {
  name:'Jumbotron'
}
</script>

<style lang="scss">
//IMPORT STYLE
@import '../assets/style/vars.scss';
@import '../assets/style/mixins.scss';


h1{
  font-family: $title-font;
  font-size: 60px !important;
  color: white;
  text-align: center;
  margin-top: 100px !important;
}
.subtitle{
  font-size: 18px;
  width: 850px;
  text-align: center;
  margin: 30px auto;
  color: white;
}

</style>