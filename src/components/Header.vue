<template>
  <header>
    <div class="container">

      <a href="#">
        <img src="../assets/img/logo-light.png" alt="logo">
      </a>

      <nav>
        <ul>
          <li v-for="(link,index) in links" :key="index">
            <a href="#">{{link}}</a>
          </li>
        </ul>
      </nav>

      <div class="icon d-flex">
        <i class="fas fa-search"></i>
        <i class="fas fa-shopping-bag"></i>
        <i class="fas fa-bars"></i>
      </div>
    </div>
    
    <Jumbotron />

  </header>
</template>

<script>

//IMPORT COMPONENTS
import Jumbotron from './Jumbotron.vue';

export default {
  components: { Jumbotron },
  name: 'Header',
  data(){
    return{
      links:[
        'Home', 
        'Courses',
        'Instructors',
        'Events',
        'Pages',
        'Elements'
      ]
    }
  }

}
</script>

<style lang="scss">
//IMPORT STYLE
@import '../assets/style/vars.scss';
@import '../assets/style/mixins.scss';


header{
  background: rgba(0, 0, 0, .3) url(../assets/img/course-9-f-img.jpg);  
  background-blend-mode: darken;
  @include background-cover;

    .container{
      @include center;
      padding-top: 30px;
      i{
        cursor: pointer;
        filter: opacity(1); 
        font-size: 20px;
        margin: 0 20px;
        color: white;
         &:first-child {
          transform: rotate(90deg);
        }
         &:hover, &:active{
          transition: all 0.3s;
          color: $primary-color;
        }
      }
      img{
          width: 250px;
        }

        ul{ 
          display: flex;
          margin: 0;

          li{
            text-transform: uppercase;
            list-style: none;
            margin: 0 20px ;

            a{
              text-decoration: none;
              color: white;
              font-size: 18px;

              &:hover{
                transition: all 0.3s;
                color: $primary-color;
              }
            }
          }
        }

    }


 
  

}

</style>