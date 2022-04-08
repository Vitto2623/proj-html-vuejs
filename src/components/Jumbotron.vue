<template>
  <div id="jumbotron">
    <!--TOP-->
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
      <div class="image-brand d-flex align-items-center">
        <div class="lay-over"></div>
        <div class="brand-description">
          <h6 class="text-white fw-bolder">FIND THE BEST ANIMAL SUPPLIES</h6>
          <p class="text-white fw-bolder animate__animated animate__fadeInLeft">We know animals are a part of your family, let us help take care of them.</p>
          <button class="border-0" id="hover">Learn more about us</button>
        </div>
      </div>
      <!--Bottom-->
      <div class="row justify-content-center align-items-center">
        <div class="col-2">
          <img src="../assets/images/food-transparent-5-200x112.png" id="size" alt="">
        </div>
        <div class="col-4 text-white">
          <span class="me-4">Get $25 OFF your first purchase of our homemade pet food!</span> <a href="#">Visit the shop</a>
        </div>
      </div>
    </div>
    <div id="mini-cards">
      <div class="my-card d-flex flex-column justify-content-center align-items-center">
        <i class="fas fa-folder"></i>
        <p>Demos</p>
      </div>
      <div class="my-card mt-1 d-flex flex-column justify-content-center align-items-center">
        <p class="fs-5" style="color: green; height: 25px;"><span style="vertical-align: super; color: green;" class="fs-6">$</span>39</p>
        <p>On sale</p>
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
@import url('https://fonts.googleapis.com/css2?family=PT+Serif:wght@400;700&display=swap');
#jumbotron{
  width: 100%;
  background-color: $color-brand;
  background-image: url('../assets/images/bg-transparent-3.png');
  .image-brand{
    position: relative;
    height: 570px;
    padding: 20px 300px;
    background-image: url('../assets/images/banner-5-2x-scaled.jpg');
    background-size: cover;
    width: 100%;
    height: 846px;
    font-family: 'PT Serif', serif;
    .brand-description{
      width: 600px;
      p{
        font-size: 2.20em;
      }
      button{
        border-radius: 30px;
        padding: 10px 30px;
        &:hover{
        background-color: #3d6f42;
        color: white;
        }
      }
    }
  }
  #size{
    width: 250px;
  }
  #mini-cards{
    position: fixed;
    top: 150px;
    right: 12px;
    cursor: pointer;
    .my-card{
      height: 45px;
      width: 45px;
      border-radius: 5px;
      background-color: lightgrey;
      p{
        font-size: 0.70em;
        margin: 0px;
        font-weight: bold;
      }
    }
  }
}
</style>