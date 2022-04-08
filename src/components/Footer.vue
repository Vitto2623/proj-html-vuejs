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
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
.footer{
  margin-top: 3160px;
  width: 100%;
  height: 700px;
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
}
</style>