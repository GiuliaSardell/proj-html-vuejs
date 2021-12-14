<template>
 <div class="container">
   <div class="row">
      <div class="col"
      v-for="(subject,index) in subjects" :key="index">
      <img :src ="require ('../assets/img/'+ subject.img)"
      :alt="subject.title">
      <span>{{subject.title}}</span>
      </div>

   </div>
   
 </div>

</template>

<script>
export default {
  name: 'Subject',
data(){
  return{
    subjects:[
      {
        title: 'Languages',
        img: 'h5-custom-icon-1.png'
      },
      {
        title: 'Software',
        img: 'h5-custom-icon-2.png'
      },
      {
        title: 'Business',
        img: 'h5-custom-icon-3.png'
      },
      {
        title: 'Chemistry',
        img: 'h5-custom-icon-4.png'
      },
      {
        title: 'Science',
        img: 'h5-custom-icon-5.png'
      },
      {
        title: 'DIY-Craft',
        img: 'h5-custom-icon-6.png'
      },

    ]
  }
}
}
</script>

<style lang="scss">

@import '../assets/style/mixins.scss';
@import '../assets/style/vars.scss';

.row{
  @include center;
  margin: 60px 0 !important;
}
.col{
  img{
    margin: 0 auto;
    margin-bottom: 20px !important;
    display: block;
  }
  cursor: pointer;
  padding: 50px 0;
  text-align: center;
  margin: 20px;
  border: 1px solid lightgray;
  background-color: #F2F8FC;
  &:hover{
    background-color: darken(#F2F8FC, 5%)
  }
  span{
    font-weight: bold;
    font-family: $title-font;
  }
 
}

</style>