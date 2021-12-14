<template>
  <div class="bg-blu">
    <div class="container container-colorSection">
      <div class="container-img">

      </div>
      <p class="p-colorSection">Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias, exercitationem dolore blanditiis fugiat voluptate magni fuga quis voluptates voluptas amet? Illo aliquam officiis animi repellendus corrupti tempore sunt asperiores sequi. Lorem, ipsum dolor sit amet consectetur adipisicing elit. Beatae asperiores necessitatibus sed, animi officiis voluptas quo suscipit nihil aliquam inventore.</p>
      <span class="student-name">Joan Collins</span>
      <span class="student">student</span>
      <div class="container-icon">
        <i class="fas fa-circle"></i>
        <i class="fas fa-circle active"></i>
        <i class="fas fa-circle"></i>
      </div>
      

      <div class="top top-colorSection">
        <a href="#">
          <i class="fas fa-chevron-up"></i>
          <span>TOP</span>
        </a>
      </div>

    </div>

    



  </div>

</template>

<script>
export default {
  name: 'ColorSection'
}
</script>

<style lang="scss">
@import '../assets/style/vars.scss';
@import '../assets/style/mixins.scss';

.bg-blu{
  background-image: url('../assets/img/h5-parallax-img-1.png');
  @include background-cover;
  background-size: 160%;
  background-position: top;
  height: 800px;
  width: 100%;
  position: relative;
  margin-bottom: 120px;

  .container-colorSection{
    @include center;
    flex-direction: column;
    padding-top: 40px;
    height: 100%;
    margin-bottom: 30px;
    .container-img{
      width: 150px;
      height: 150px;
      background-image: url('../assets/img/instructor-img-6.jpg');
      background-size: 160%;
      background-position: 60% 25%;
      border-radius: 50%;
    }

    .p-colorSection{
      color: white;
      width: 1000px;
      line-height: 40px;
      text-align: center;
      margin: 40px 0 20px 0;
    }

    .student-name{
      color: white;
      font-size: 30px;
      font-family: $title-font;
      display: block;
      margin: 20px 0;
    }

    .student{
      color: white;
      text-transform: uppercase;
      font-size: 18px;
    }

    .container-icon{
      margin-top: 100px;
      i{
        color: white;
        margin: 10px;
        filter: opacity(.5);
      }

      .active{
        filter: none;
      }

    }

    .top-colorSection{
      position: absolute;
      right: 0;
      top: 105%;
    }
 
  }
}


</style>