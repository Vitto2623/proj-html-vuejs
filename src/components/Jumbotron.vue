<template>
  <div id="jumbotron">
    <div class="container-fluid px-0">
      <div class="row text-white justify-content-center py-3">
        <div class="col-3 text-center">
          <span class="fw-bold"><i class="fas fa-map"></i> International</span> <span>Shipping Services</span>
        </div>
        <div class="col-3 text-center">
          <span><i class="fas fa-clock"></i> See our </span> <span class="fw-bold">store hours</span> <span>and services</span>
        </div>
        <div class="col-3 text-center">
          <span><i class="fas fa-check"></i> We price match to give you the </span> <span class="fw-bold"> best deals</span>
        </div>
      </div>
      <div class="image-brand">
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name : 'IndexJumbotron'
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
#jumbotron{
  width: 100%;
  background-color: $color-brand;
  background-image: url('../assets/images/bg-transparent-3.png');
  .image-brand{
    height: 570px;
    background-image: url('../assets/images/banner-5-2x-scaled.jpg');
    background-size: cover;
    width: 100%;
    height: 846px;
    position: relative;
  }
  .image-brand::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0,0,0,0.3);
  }
}
</style>