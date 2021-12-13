<template>
  <div class="container">
    
    <h2>The Trusted Name for In-Home Tutoring.</h2>
    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sunt quo impedit excepturi inventore id exercitationem voluptates omnis, consectetur dicta fuga. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsa, sed. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Rerum, voluptatibus?</p>
    <a class="link-blue" href="#">Learn more</a>


    <img src="../assets/img/h5-img-1.jpg" alt="img">

    <div class="top">
      <a href="#">
        <i class="fas fa-chevron-up"></i>
        <span>TOP</span>
      </a>
      
    </div>

    
  </div>
</template>

<script>
export default {
  name: 'Section'
}
</script>

<style lang="scss">
@import '../assets/style/vars.scss';
@import '../assets/style/mixins.scss';

.container{
  position: relative;
  
  h2{
    width: 400px;
    font-family: $title-font;
    font-weight: bold !important;
    margin-bottom: 20px !important;
  }
  p{
    font-size: 18px;
    color: grey;
  }
  .link-blue{
    margin: 25px 0;
    display: block;
    text-transform: uppercase;
    font-weight: bold;
    text-decoration: none !important;
    color: $primary-color !important;
    &:hover{
      color: darken($primary-color, 20% )!important;
    }
  }

  .top{
    i{
      display: block;
      font-size: 30px;
    }
    @include center (both);
    flex-direction: column;
    cursor: pointer;
    color: white;
    font-size: 20px;
    width: 80px;
    height: 80px;
    background-color: $primary-color;
    position: absolute;
    right: 0;
    top: 70%;
    &:hover{
      color: darken($primary-color, 20% )!important;
    }

    a{
      text-decoration: none;
      text-align: center;
      color:white;
      &:hover{
      color: darken($primary-color, 20% )!important;
      transition: all 0.3s;
    }
    }

   
  }
}

</style>