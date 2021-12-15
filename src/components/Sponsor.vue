<template>
  <div class="sponsor">

    <div class="top top-patternSection">
        <a href="#">
          <i class="fas fa-chevron-up"></i>
          <span>TOP</span>
        </a>
      </div>

  <div class="container container-sponsor">


    <img src="../assets/img/h5-client-5.png" alt="">
    <img src="../assets/img/h5-client-1.png" alt="">
    <img src="../assets/img/h5-client-2.png" alt="">
    <img src="../assets/img/h5-client-1.png" alt="">




  </div>
</div>

</template>

<script>
export default {
  name: 'Sponsor'
}
</script>

<style lang="scss">

.sponsor{
  height: 150px;
  position: relative;

  img{
    margin: 120px 0;
  }

  .top{
    position: absolute;
    right: 0;
    top: 5px;
  }
}

</style>