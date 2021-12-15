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
              <tr>
                
              </tr>
            </thead>
            <tbody
            v-for="(box, index) in tableBoxes" :key="index">
              <tr>
                <td>
                {{box.col1}}
                </td>
                <td>{{box.col2}}</td>
                <td>{{box.col3}}</td>
                <td>{{box.col4}}</td>
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
      tableBoxes:[

        {
          col1:'Save up to 40% by paying weekly',
          col2:['img','Number of Courses','$12'],
          col3: 'col3row3',
          col4: 'col4row4'
        },
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

.container-plans{
  .top-plans{
    text-align: center;
    margin: 50px 0;
    h2{
      font-family: $title-font;
      font-weight: bold;
    }
  }

}




</style>