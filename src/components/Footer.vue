<template>
  <footer>
    <div class="container container-footer " >
      <div class="footer-flex d-flex py-5 justify-content-center">

        <div class="lista1 " style="width: 350px">            
          <ul >
            <li class="my-4">
              <img src="../assets/img/footer-logo-1.png" alt="">
            </li>
            <li v-for="(item,indice) in items" :key="indice">
              {{ item }}
            </li>

          </ul>
          <div class="contact d-flex flex-column mx-3" style="margin-top: 50px">
            <span><i class="fas fa-phone"></i> 1-677-124-44227</span>
            <span><i class="far fa-clock"></i> Mon - Sat 8.00 - 18.00</span>
          </div>
        </div>

        <div class="lista2" style="width: 300px ">
          <ul>
            <li class="my-4">
              <h2>Popular Courses</h2>
            </li>
            <li v-for="(item,indice) in items2" :key="indice">
              {{ item }}
            </li>
          </ul>
        </div>

        <div class="lista3" style="width: 200px">
          <ul>
            <li class="my-4">
              <h2>Support</h2>
            </li>
            <li v-for="(item,indice) in items3" :key="indice">
              {{ item }}
            </li>
          </ul>
        </div>

        <div class="lista4" style="width: 350px">
          <ul>
            <li class="my-4">
              <h2>Flexible Learning</h2>
            </li>
            <li v-for="(item,indice) in items4" :key="indice">
              <img :src ="require ('../assets/img/'+ item)"
            :alt="mappa"
            style="width: 300px">
              
            </li>
          </ul>
        </div>

      </div>

      <div class="copyright d-flex justify-content-lg-between py-5">
        <span>
          Copyrights 2017 Mikado Themes
        </span>
        <div class="social d-flex">
          <span class="mx-3">CALL +44 300 303 0266</span> 
          <span>FOLLOW US</span> 
          <span><i class="fab fa-twitter"></i></span>
          <span><i class="fab fa-instagram"></i></span>
          <span><i class="fab fa-facebook-square"></i></span>

        </div>

        
        
      </div>

      <div class="top top-patternSection">
        <a href="#">
          <i class="fas fa-chevron-up"></i>
          <span>TOP</span>
        </a>
      </div>

      
    </div>
  </footer>
</template>

<script>
export default {
  data(){
    return{
      items:['Providing Life Changing Experiences Throught Education, Class That Fit Your Busy Life. Closer to Home' ],

      items2:[ 'Business English', 'Preston Marshall', 'Social Computing', 'David Sanders', 'Learn Spanish', 'Jennie King'],
      items3:[ 'User dashboard', 'Contact Us', 'FAQ', 'Course Offer', 'Events'],
      items4:[ 'footer-img-1.png'],

    }
  }

}
</script>

<style lang="scss">
//IMPORT STYLE
@import '../assets/style/vars.scss';
@import '../assets/style/mixins.scss';

footer{
  position: relative;
  margin-top: 150px;
  background-color: #222222;
  color: grey;
  font-size: 17px;
  
  
  .top{
      position: absolute;
      bottom: 0;
      right: 0;
  }  

    
  

  .footer-flex{
    ul{
      list-style-type: none;
      li{
        cursor: pointer;
        &:hover{
          color: lightgrey;
        }
        h2{
          font-family: $title-font;
          color: white;
        }
      }
    }

    margin-bottom: 30px;
    border-bottom: 2px solid lightgrey;
  }

  .copyright{
    span{
      font-size: 14px;
      margin: 0 10px;
    }
  }
  
}

</style>