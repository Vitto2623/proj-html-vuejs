<template>
  <div>
    <div class="footer">
      <div id="top-footer">
        <div id="top" class="d-flex  justify-content-between">
          <nav>
            <a href="#">
              <img src="../assets/images/mobile-light-pet-logo-2x.png" alt="">
            </a>
            <ul class="text-white list-unstyled mt-4">
              <li v-for="(element, index) in NavLinks1" :key="'primo'+index">
                <a href="#" class="text-decoration-none text-white">{{element.text}}</a>
              </li>
            </ul>
          </nav>
          <nav class="text-white" style="width: 242px;">
            <ul class="list-unstyled">
                <h5>Shop by brand</h5>
              <li v-for="(element, index) in NavLinks2" :key="'secondo'+index" class="mt-4">
                <a href="#" class="text-decoration-none text-white">{{element.text}}</a>
              </li>
            </ul>
          </nav>
          <nav class="text-white" style="width: 246px;">
            <ul class="list-unstyled">
              <h5>Useful links</h5>
              <li v-for="(element, index) in NavLinks3" :key="'terzo'+index" class="mt-4">
                <a href="#" class="text-decoration-none text-white">{{element.text}}</a>
              </li>
            </ul>
          </nav>
          <form action="#">
            <div id="news-letter" class="rounded-3 d-flex flex-column">
              <h5 class="text-white">Subscribe to our newsletter</h5>
              <input type="email" placeholder="Insert your email...*" class="border-0 bg-white">
              <button class="border-0 text-white mt-4">Subscribe</button>
            </div>
          </form>
        </div>
        <div id="bottom" class=" d-flex justify-content-center flex-column align-items-center">
          <nav>
            <ul class="d-flex mt-5">
              <li class="mx-3 list-unstyled" v-for="(element, index) in NavLinks4" :key="'quarto'+index">
                <a href="#" class="text-decoration-none text-white">{{element.text}}</a>
              </li>
            </ul>
          </nav>
          <nav class="d-flex justify-content-center">
            <a href="#"><i class="fab fa-facebook-f m-3 text-white"></i></a>
            <a href="#"><i class="fab fa-twitter m-3 text-white"></i></a>
            <a href="#"><i class="fab fa-instagram m-3 text-white"></i></a>
            <a href="#"> <i class="fab fa-youtube m-3 text-white"></i></a>
          </nav>
        </div>
      </div>
      <div id="bottom-footer" class="text-center">
        <h6 class="text-white">© Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress</h6>
        <form action="#">
          <button id="go-up">
            <i class="fas fa-angle-up text-white"></i>
          </button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name : 'IndexFooter',
    data: function(){
      return{
        NavLinks1 : [
          {
            text: '1234 Avada Avenue Avadaville',
          },
          {
            text: 'info@your-company.com',
          },
          {
            text: 'Call us: (1) 234 5678'
          }
        ],
        NavLinks2 : [
          {
            text: 'Bed',
          },
          {
            text: 'Food',
          },
          {
            text: 'Toys',
          },
          {
            text: 'Transport'
          }
        ],
        NavLinks3: [
          {
            text: 'My account'
          },
          {
            text: 'Orders'
          },
          {
            text: 'Checkout'
          },
          {
            text: 'Cart'
          }
        ],
        NavLinks4:[
          {
            text: 'Home'
          },
          {
            text: 'About'
          },
          {
            text: 'Blog'
          },
          {
            text: 'Contact'
          },
          {
            text: 'Shop'
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
.footer{
  margin-top: 3160px;
  width: 100%;
  background-color: lightgrey;
  #top-footer{
    background-color: #253025;
    width: 100%;
    height: 92%;
    padding: 100px 330px;
    #top{
      border-bottom: 1px solid rgb(2, 72, 2);
      padding: 0px 0px 50px 0px;
      img{
        width: 218px;
      }
      form{
        width: 239px;
      }
      #news-letter{
        width: 239px;
        height: 248px;
        background-image: url('../assets/images/bg-transparent-3.png');;
        background-size: 300px;
        background-color: #264229;
        padding: 34px 24px 0px 24px;
        input{
          border-radius: 50px;
          padding: 10px;
          margin-top: 23px;
        }
        button{
          border-radius: 50px;
          padding: 10px;
          background-color: #3d6f42;
        }
      }
    }
  }
  #bottom-footer{
    background-color: black;
    width: 100%;
    height: 66px;
    position: relative;
    h6{
      line-height: 66px;
    }
    form{
      position: absolute;
      bottom: 0px;
      right: 55px;
      #go-up{
        width: 34px;
        height: 33px;
        background-color: #2e2e2e;
        border-top-left-radius: 5px;
        border-top-right-radius: 5px;
        border: none
      }
    }
  }
}
</style>