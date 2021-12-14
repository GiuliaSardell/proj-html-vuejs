<template>
  
   <div class="section-pattern">
    <div class="container container-pattern">

      <div class="pattern-top flex-column">
        <h2>Popular Online Courses</h2>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quibusdam dolorum ea aliquam voluptate dolores. Possimus reiciendis dolores excepturi laudantium voluptatem?</p>
      </div>
    

      <div class="pattern-bottom d-flex justify-content-center">
        <div class="card mx-3"
        v-for="(element, index) in elements" :key="index">
      
          <img :src ="require ('../assets/img/'+ element.img)"
          :alt="element.role">

          <div class="linear">
            <span class="role">{{element.role}}</span> 
            <span class="cost">{{element.cost}}</span>
          </div>
          
          <span class="name">{{element.name}}</span>
          <p>{{element.description}}</p>

          <div class="icon-pattern">
            <i class="fas fa-user"></i> <span class="users">{{element.users}}</span>
            <i class="fas fa-tag"></i> <span class="program">{{element.program}}</span>
          </div>
         

        </div>

      </div>

    </div>
   </div>
</template>

<script>
export default {
  name: 'PatternSection',
  data(){
    return{
      elements:[
        {
          img: 'course-5-f-img.jpg',
          role: 'Android Developer',
          cost: 'Free',
          name: 'David Sanders',
          description: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur sint nemo necessitatibus. Distinctio doloribus aut maxime impedit molestias minus dolore!',
          users: '1',
          program: 'programming'
        },
        {
          img: 'course-6-f-img.jpg',
          role: 'Web Designing',
          cost: 'Free',
          name: 'Jennifer Powell',
          description: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur sint nemo necessitatibus. Distinctio doloribus aut maxime impedit molestias minus dolore!',
          users: '1',
          program: 'programming'
        },
        {
          img: 'course-12-f-img.jpg',
          role: 'Financial Modelin',
          cost: '$20',
          name: 'Edward Bowman',
          description: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Consequatur sint nemo necessitatibus. Distinctio doloribus aut maxime impedit molestias minus dolore!',
          users: '1',
          program: 'business'
        }
      ]
    }
  }
}
</script>

<style lang="scss">
@import '../assets/style/vars.scss';
@import '../assets/style/mixins.scss';

.section-pattern{

  .pattern-top{
    @include center;
    margin-bottom: 60px;
    

    h2{
      font-family: $title-font;
      font-size: 35px;
      font-weight: bold;
    }
    p{
      text-align: center;
    }
  }

  .pattern-bottom{
    .card{
      width: 301px;
      border: 1px solid lighter($secondary-color, 30%);
      border-radius: 0;
      img{
        width: 100%;
      }
      .linear{
        margin: 10px 0;
        display: flex;
        justify-content: space-around;
        .role{
        font-family: $title-font;
        font-weight: bold;
        
      }
      .cost{
        text-align: center;
        text-transform: uppercase;
        color: white;
        background-color: #FFD740;
        padding: 2px 10px;
        border-radius: 10px;
        width: 55px;
      }
      }
      

      .name{
        font-size: 16px;
        font-weight: bold;
        color: $secondary-color;
        margin: 0 20px;
      }
      p{
        font-size: 14px;
        color: $secondary-color;
        margin: 10px 20px;

      }

      .icon-pattern{
        display: flex;
        margin: 0 20px;
        align-items: center;
        .users, .program, i{
          margin:5px;
          color: $secondary-color;
          text-transform: uppercase;
          font-weight: bold;
        }


      }

      

    }
  }
}
</style>