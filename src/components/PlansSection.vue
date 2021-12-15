<template>
 <div class="section-plans">
    <div class="container container-plans">

      <div class="top-plans">
        <h2>Pricing Plans</h2>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quibusdam dolorum </p>
      </div>
      
      <div class="bottom-plans table">

        <div class="table-responsive">
          <table class="table align-middle"
          >
            <thead
            >
              <tr class="title-row"> 
                <td
                v-for="(title, i) in titleBox" :key="i">
             

                  <!-- <img src="../assets/img/h5-custom-icon-7.png" alt="">
                  <img :src ="title.img" :alt="title.title"> -->
                  <!-- <img :src="require(`../assets/img/${title.img}`)" alt class="title.title" /> -->
                  <!-- <img :src="'/img/' + title.img + '.png'" v-bind:alt="title.title" > -->
                  <!-- <img :src=" require('../assets/img/' + title.img + '.png')" v-bind:alt="title.title" > -->
                  <!-- <img :src =" require('../assets/img/' + title.img )"  :alt="title.title"> -->

                  <div class="container-title d-flex flex-column justify-content-center align-items-center my-4 ">
                    <img class="" src="../assets/img/h5-custom-icon-7.png" alt="">

                    <div class="title">
                      {{title.title}}
                    </div>

                    <div class="title-cost">
                      {{title.cost}}
                    </div>

                  </div>
                  
 

                  
                  
                  
                  
                </td>
              </tr>
            </thead>
            <tbody
            >
              <tr v-for="(box, index) in tableBoxes" :key="index">
                <td>
                {{box.col1}}
                </td>
                <td  style="text-align: center">{{box.col2}}</td>
                <td  style="text-align: center">{{box.col3}}</td>
                <td  style="text-align: center">{{box.col4}}</td>
                
              </tr>
              
            </tbody>
          </table>
        </div>

      </div>

    </div>
    
  </div>


</template>

<script>
export default {
  name: 'PlansSection',
 
  data(){
    return{

      titleBox:[
        { 
          img: '',
          title:'Save up to 40% by paying weekly',
          cost: '_'
        },
        {
          img: 'h5-custom-icon-7.png',
          title:'Standard',
          cost: '$12'
        },
        {
          img: 'h5-custom-icon-8.png',
          title:'Professional',
          cost: '$12'
        },
        {
          img: 'h5-custom-icon-9.png',
          title:'Advanced',
          cost: '$12'  
        }
      ],
      tableBoxes:[
        {
          col1:'Number of Courses',
          col2: '2',
          col3: '4',
          col4: '6'
        },
        {
          col1: 'Time',
          col2: '15 Days',
          col3: '30 Days',
          col4: '30 Days'
        },
        {
          col1: 'Web Designer',
          col2: '✓',
          col3: '✓',
          col4: '✓',
        },
        {
          col1: 'Human-Centered Design',
          col2: '✓',
          col3: '✓',
          col4: '✓',
        },
        {
          col1: 'Basic Marketing',
          col2: '✗',
          col3: '✓',
          col4: '✓',
        },
        {
          col1: 'Phyton for Everybody',
          col2: '✗',
          col3: '✓',
          col4: '✓',
        },
        {
          col1: 'Android Developer',
          col2: '✗',
          col3: '✗',
          col4: '✓',
        },
        {
          col1: 'Business English',
          col2: '✗',
          col3: '✗',
          col4: '✓',
        },
  
      ],
     
    }
  }
}
</script>

<style lang="scss">

@import '../assets/style/vars.scss';
@import '../assets/style/mixins.scss';

.section-plans{
  border-bottom: 2px solid lightgrey;

}

.container-plans{
  .top-plans{
    text-align: center;
    margin: 50px 0;
    h2{
      font-family: $title-font;
      font-weight: bold;
    }
  }

  .table{
    margin-bottom: 70px;
    thead{
      font-weight: bold;
      background-color: #F7FDFF;
      
      .title-row{
        &:first-child{
          width: 230px;
        }
      }

      td{
        border-left: 1px solid lightgrey;
        border-right: 1px solid lightgrey;
        border-top: 4px solid #D4F2FF;
        cursor: pointer;
        &:hover, &:active{
        border-top: 4px solid $primary-color;

        }
      }
    }
    tbody{
      tr{
        line-height: 50px;
        td{
          border-left: 1px solid lightgrey;
          border-right: 1px solid lightgrey;
        }
        
        
      }
    }
    font-family: $title-font;
  }
  
}




</style>