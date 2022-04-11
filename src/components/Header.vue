<template>
  <div>
    <!--TOP HEADER-->
    <div class="my-container">
      <div class="container-fluid text-center py-2 top-header">
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
    <div class="bottom-header py-2">
      <!--NAV-BAR-->
      <nav>
        <ul class="d-flex justify-content-center list-unstyled mb-0">
          <li v-for="(link, index) in HeaderLinks" :key="'primo'+index" class="d-flex justify-content-center align-items-center">
            <div class="dropdown" id="menù">
              <button href="#" class="m-3 text-decoration-none fw-bold border-0 btn btn-success" type="button" id="dropdownMenuButton1" data-bs-toggle="dropdown" aria-expanded="false" :class="{active: link.current}">{{link.text}}<span class="fas fa-angle-down ms-2"></span></button>
                <li class="menu dropdown-menu bg-black" aria-labelledby="dropdownMenuButton1"><a class="dropdown-item my-bg" href="#"  v-for="(link, index) in  NavToggleMenu" :key="'secondo'+index">{{link.text}}</a></li>
            </div>
          </li>
          <li v-for="(element, index) in HeaderLinksSpecial" :key="'secondo'+index" class="d-flex justify-content-center align-items-center">
            <div class="dropdown">
              <button href="#" class="m-3 text-decoration-none  fw-bold border-0 btn btn-secondary" type="button" id="dropdownMenuButton1" data-bs-toggle="dropdown" aria-expanded="false" >{{element.text}}</button>
              <li class="menu dropdown-menu dropdown-menu-end bg-black" aria-labelledby="dropdownMenuButton1"><a class="dropdown-item  my-bg" href="#" v-for="(link, index) in  NavToggleMenu2" :key="'terzo'+index">{{link.text}}</a></li>
            </div>
          </li>
        </ul>
      </nav>
      <!--/ NAV-BAR-->
    </div>
  </div>
</template>

<script>
export default {
    name : 'IndexHeader',
    data: function () {
    return {
      HeaderLinks: [
        {
          text: 'Home',
          url: '#',
          current: true
        },
        {
          text: 'Shop',
          url: '#',
        },
        {
          text: 'Shop My Brand',
          url: '#',
        }
      ],
      HeaderLinksSpecial: [
        {
          text: 'About',
          url: '#',
        },
        {
          text: 'Blog',
          url: '#'
        },
        {
          text: 'Contact',
          url: '#'
        }
      ],
      NavToggleMenu: [
        {
          text: 'Sezione Prodotti',
        },
        {
          text: 'Lavora con noi',
        },
        {
          text: 'Chi siamo',
        }
      ],
      NavToggleMenu2: [
        {
          text: 'Dove siamo',
        },
        {
          text: 'Politiche aziendali',
        },
        {
          text: 'Pets 2.0',
        }
      ]
    };
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
.my-container{
  border-bottom: 1px solid lightgrey;
}
div.top-header{
  padding: 0px 200px;
}
div.bottom-header{
  height: 55px;
  .fa-angle-down{
    font-size: 12px;
    vertical-align: baseline;
  }
  ul{
    height: 40px;
    li{
      button{
        color: grey;
        background: border-box;
        &.active,
        &:hover{
          color: black;
        }
      }
    }
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

@keyframes mymove {
  from {top: -29px;}
  to {top: 0px;}
}

.menu{
  width: 800px;
  animation: mymove 0.90s ease-out;
  font-size: 1.10em;
  border-radius: 12px;
}

.my-bg{
  background-color: $color-brand;
  color: white;
}
</style>