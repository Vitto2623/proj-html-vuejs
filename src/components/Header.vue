<template>
  <div>
    <!--TOP HEADER-->
    <div class="my-container">
      <div class="container-fluid text-center py-2 my-header">
        <div class="row justify-content-center  align-items-center">
          <div class="col-3">
            <img src="../assets/images/dark-pet-logo.png" alt="Brand-logo">
          </div>
          <div class="col-3">
            <div id="wrap" class="d-flex justify-content-between ms-5">
              <img src="../assets/images/lens-copia.svg" alt="">
              <input type="search" name="Search" id="SearchBar" placeholder="Search..." class="border-0">
            </div>
          </div>
          <div class="col-4">
            <span><span class="text-black fw-bold">Questions?</span> Call us : 1.800.123.4567</span>
          </div>
          <div class="col-1">
            <i class="fas fa-bag-shopping me-2"></i>
            <i class="fas fa-user"></i>
          </div>
        </div>
    </div>
    </div>

    <!---BOTTOM HEADER-->
    <div class="my-header py-2">
      <nav>
        <ul class="d-flex justify-content-center list-unstyled">
          <li>
            <a href="#" class="m-4 text-decoration-none text-dark">prova<span class="fas fa-angle-down ms-1"></span></a>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
    name : 'IndexHeader'
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
.my-container{
  border-bottom: 1px solid lightgrey;
}
div.my-header{
  width: $width;
  min-width: $min-width;
  .fa-angle-down{
    font-size: 12px;
    vertical-align: baseline;
  }
}
#wrap{
  background-color: #f3f4f3;
  border-radius: 50px;
  img{
    width: 3em;
    padding: 15px;
  }
  #SearchBar{
    background-color: #f3f4f3;
    border-radius: 50px;
    width: 600px;
  }
}
</style>