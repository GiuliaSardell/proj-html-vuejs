<template>
  <div class="jumbotron">
    
    <h1>
      Contemporary Ideas
    </h1>
    <div class="subtitle">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus distinctio reiciendis et laudantium odit aperiam ut impedit maxime optio sed dolorem, accusantium saepe.
    </div>

    <button>REGISTER NOW</button>

    <div class="icon">
      <i class="fas fa-circle"></i>
      <i class="fas fa-circle"></i>
      <i class="far fa-dot-circle"></i>
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

.jumbotron{
  display: flex;
  flex-direction: column;
}
h1{
  font-family: $title-font;
  font-size: 60px !important;
  color: white;
  text-align: center;
  margin-top: 120px !important;
}
.subtitle{
  font-size: 18px;
  width: 850px;
  text-align: center;
  margin: 30px auto;
  color: white;
}
button{
  background-color: $primary-color;
  border: none;
  // border-color: $primary-color;
  padding: 15px 25px;
  color: white;
  text-transform: uppercase !important;
  width: 200px;
  margin: 30px auto !important;
  margin-bottom: 120px !important;
  &:hover{
    background-color: darken($primary-color, 30%);
    transition: all 0.3s;
  }
}
.icon{
  text-align: center;
  padding: 30px;

  i{
    cursor: pointer;
    color: white;
    margin: 0 10px;
    font-size: 20px;
    filter: opacity(.5); 
    &:hover{
      filter: none;
      transition: all 0.3s;
    }
    // padding-top: 120px;
  }
} 

</style>