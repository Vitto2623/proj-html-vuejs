<template>
  <main>
      <div class="container-fluid text-center p-5">
        <div class="row p-5">
          <div class="col-12">
            <h2>Browse by category</h2>
            <p class="fs-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Fugit, atque inventore odio, ipsa numquam possimus earum blanditiis illo sed reprehenderit libero eligendi consequuntur eum quidem non aspernatur et, molestias quos.</p>
          </div>
        </div>
      </div>
      <!--Articoli-per-cani-->
      <div class="container-fluid animate__animated animate__fadeInDown animate__delay-2s">
        <div class="row justify-content-center mb-5">
            <div class="col-2 d-flex flex-column align-items-center mb-5" v-for="(element, index) in product" :key="'primo'+index">
                  <div class="item-card">
                    <div class="container-overlay">
                      <img :src="require(`../assets/images/${element.image}`)" alt="" class="image">
                      <div class="overlay">
                        <a href="#" class="icon text-decoration-none">
                          <i class="fas fa-check"></i>
                          <h6>VIEW CART</h6>
                        </a>
                      </div>
                    </div>
                  </div>
                  <h5 class="mt-4">{{element.name}}</h5>
            </div>
        </div>
      </div>
      <!--Food-Section-->
      <div class="my-container animate__animated animate__bounceInUp animate__delay-2s">
        <div class="food-card d-flex flex-column text-center align-items-center justify-content-center" v-for="(element, index) in food" 
        :key="'secondo'+index">
          <h1>{{element.name}}</h1>
          <h6>{{element.type}}</h6>
          <img :src="require(`../assets/images/${element.image}`)"  alt="foods-products">
          <button class="border-0">{{element.shop}}</button>
        </div>
      </div>
      <!---->
      <div class="arrivals-weekly animate__animated animate__fadeInDown animate__delay-3s">
        <div class="lay-over"></div>
        <h6 class="text-white mb-4">FIND THE BEST ANIMAL SUPPLIES</h6>
        <h2 class="text-white fs-1 fw-bolder mb-4">New arrivals weekly</h2>
        <button class="border-0">Learn more about us</button>
      </div>
      <div class="container-fluid">
        <div class="row my-row mt-5">
          <!--Top-section-->
          <div class="top d-flex justify-content-between align-items-center mt-5 animate__animated animate__fadeInDown animate__delay-3.5s">
            <div>
              <h6>All-time best sellers</h6>
              <h3>Items everyone loves</h3>
            </div>
            <button class="border-0">View all products</button>
          </div>
        </div>
        <!--Bottom-section-->
        <div class="row justify-content-center mt-5 animate__animated animate__fadeInDown animate__delay-4s">
          <div class="col-2 m-1 d-flex flex-column align-items-center" v-for="(element, index) in product2" :key="'terzo' +index">
            <div class="item-card d-flex align-items-center justify-content-center">
                <div class="container-overlay">
                  <img :src="require(`../assets/images/${element.image}`)" alt="products" class="image">
                  <div class="overlay">
                    <a href="#" class="icon text-decoration-none">
                      <i class="fas fa-check"></i>
                      <h6>VIEW CART</h6>
                    </a>
                  </div>
                </div>
            </div>
            <h5 class="mt-3">{{element.name}}</h5>
            <h5 style="color: #3d6f42;" class="fs-6">{{element.price}}</h5>
          </div>
        </div>
      </div>
      <!--Section-of-Users-testimonials-->
      <div class="container-fluid p-0" id="users-testimonials">
        <div class="row text-center">
          <div class="col-12 mt-5">
            <h1 class="text-white">Users testimonials</h1>
          </div>
        </div>
        <div class="row justify-content-center text-center mt-5 px-5">
          <div class="col-3 px-5">
            <img src="../assets/images/avatar-3-200x200.jpg" class="img-fluid rounded-circle w-25" alt="user-image">
            <p class="p-0 mt-3 text-white">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repellendus, iusto autem veritatis qui doloribus facere in culpa velit, nisi ea maxime incidunt architecto libero placeat dolorum nostrum voluptas deleniti odit?</p>
            <h6>Lisa Smith, ThemeFusion</h6>
          </div>
          <div class="col-3 px-5">
            <img src="../assets/images/avatar-1-200x200.jpg" class="img-fluid rounded-circle w-25" alt="user-image">
            <p class="p-0 text-white mt-3">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repellendus, iusto autem veritatis qui doloribus facere in culpa velit, nisi ea maxime incidunt architecto libero placeat dolorum nostrum voluptas deleniti odit?</p>
            <h6>Melissa Green, ThemeFusion</h6>
          </div>
          <div class="col-3 px-5">
            <img src="../assets/images/avatar-4-200x200.jpg" class="img-fluid rounded-circle w-25" alt="user-image">
            <p class="p-0 mt-3 text-white">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repellendus, iusto autem veritatis qui doloribus facere in culpa velit, nisi ea maxime incidunt architecto libero placeat dolorum nostrum voluptas deleniti odit?</p>
            <h6>Sam Lewis, ThemeFusion</h6>
          </div>
        </div>
        <!--Form-->
        <div id="form" class="animate__animated animate__fadeInDown animate__delay-4.5s">
          <form action="#">
            <h2>Join our newsletter</h2>
            <p class="p-0 mt-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel recusandae tempore deserunt aliquam non dignissimos corrupti itaque suscipit ullam quasi! Ipsam eius fugiat soluta accusamus ex delectus exercitationem, quam earum.</p>
            <div class="d-flex">
              <input type="email" placeholder="Insert your email...*" class="border-0">
              <button class="border-0 ms-3">Subscribe</button>
            </div>
          </form>
        </div>
        <!--Recent-articles-->
        <div class="container-fluid animate__animated animate__fadeInDown animate__delay-5s">
          <div class="row text-center mt-5">
            <div class="col-12">
              <h2>Get the best tips & tricks</h2>
              <h6>Recent articles</h6>
            </div>
          </div>
          <div class="row justify-content-center mt-5">
            <div class="col-2 m-1 d-flex flex-column align-items-center" v-for="(element, index) in articles" :key="'quarto' +index">
              <div class="item-card">
                <div class="container-overlay">
                  <img :src="require(`../assets/images/${element.image}`)" alt="articles">
                  <div class="overlay d-flex justify-content-center align-items-center px-5">
                    <a href="#" class="text-decoration-none">
                      <h6 class="text-white fs-3">{{element.overText}}</h6>
                    </a>
                  </div>
                </div>
                <!--Product-description-->
                <div class="p-4">
                  <h5>{{element.text}}</h5>
                  <h6 class="text-grey">{{element.date}}</h6>
                </div>
              </div>
            </div>
          </div>
          <div class="row text-center mt-5">
            <div class="col-12" style="margin-top: 100px;">
              <button class="border-0">Read all articles</button>
            </div>
          </div>
        </div>
        <!---->
        <div id="section-of-best-products" class="animate__animated animate__fadeInDown animate__delay-5.5s animate__slower	">
          <div class="d-flex">
            <div id="left-image" class="d-flex flex-column align-items-center justify-content-center animate__animated animate__fadeInDown animate__delay-5.5s animate__slower	">
              <div class="lay-over"></div>
              <h6 class="text-white">FIND THE BEST ANIMAL SUPPLIES</h6>
              <h2 class="text-white mt-3">Popular accessories</h2>
              <button class="border-0 mt-3">View all toys accessories</button>
            </div>
            <div id="right-image" class="d-flex flex-column align-items-center justify-content-center animate__animated animate__fadeInDown animate__delay-5.5s animate__slower	">
              <div class="lay-over"></div>
              <h6 class="text-white">FIND THE BEST FOOD</h6>
              <h2 class="text-white mt-3">New food arrival</h2>
              <button class="border-0 mt-3">View all food arrival</button>
            </div>
          </div>
          <div class="container-fluid text-center">
            <div class="row justify-content-center align-items-center" style="height: 340px">
              <div class="col-2">
                <i class="fas fa-truck fs-1 text-white"></i>
                <h6 class="mt-4">Free worldwide deliveries</h6>
              </div>
              <div class="col-2 m-1">
                <i class="fas fa-map fs-1 text-white"></i>
                <h6 class="mt-4">Find stores near you</h6>
              </div>
              <div class="col-2 m-1">
                <i class="fas fa-dollar-sign fs-1 text-white"></i>
                <h6 class="mt-4">Best prices guarranteed</h6>
              </div>
              <div class="col-2">
                <i class="fas fa-credit-card fs-1 text-white"></i>
                <h6 class="mt-4">All credit card accepted</h6>
              </div>
            </div>
          </div>
        </div>
        <div class="container-fluid animate__animated animate__fadeInDown animate__delay-5.5s">
          <div class="row text-center mt-5">
            <div class="col-12">
              <h2>New products arrival</h2>
              <h6>Latest products</h6>
            </div>
          </div>
          <!--Top-->
          <div class="row justify-content-center mt-4">
            <div class="col-2 d-flex flex-column align-items-center">
              <div class="item-card-2 mb-4">
                <div class="container-overlay">
                  <img src="../assets/images/product-8-500x500.jpg" class="img-fluid" alt="">
                  <div class="overlay">
                    <a href="#" class="icon text-decoration-none">
                      <i class="fas fa-check"></i>
                      <h6 class="text-white">VIEW CART</h6>
                    </a>
                  </div>
                </div>
              </div>
              <h6 class="text-black">Colored pet bed</h6>
              <h6>$18.00 - $26.00</h6>
            </div>
            <div class="col-2 d-flex flex-column align-items-center">
              <div class="item-card-2 mb-4">
                <div class="container-overlay">
                  <img src="../assets/images/product-2-500x500.jpg" class="img-fluid" alt="">
                  <div class="overlay">
                    <a href="#" class="icon text-decoration-none">
                      <i class="fas fa-check"></i>
                      <h6 class="text-white">VIEW CART</h6>
                    </a>
                  </div>
                </div>
              </div>
              <h6 class="text-black">Dog bone</h6>
              <h6>$29.00</h6>
            </div>
            <div class="col-2 d-flex flex-column align-items-center">
              <div class="item-card mb-4">
                <div class="container-overlay">
                  <div id="special" class="rounded-circle">Sale!</div>
                  <img src="../assets/images/product-3-500x500.jpg" class="img-fluid" alt="">
                  <div class="overlay">
                    <a href="#" class="icon text-decoration-none">
                      <i class="fas fa-check"></i>
                      <h6 class="text-white">VIEW CART</h6>
                    </a>
                  </div>
                </div>
              </div> 
              <h6 class="text-black mt-5">Dog bone</h6>
              <h6>$̶2̶9̶.̶0̶0̶ $18.00</h6>
            </div>
          </div>
          <!--Bottom-->
          <div class="row justify-content-center mt-5">
            <div class="col-2 d-flex flex-column align-items-center" v-for="(element, index) in articles2" :key="'quinto' +index">
              <div class="item-card-2 mb-4">
                <div class="container-overlay">
                  <img :src="require(`../assets/images/${element.image}`)" class="img-fluid" alt="articles">
                  <div class="overlay">
                    <a href="#" class="icon text-decoration-none">
                      <i class="fas fa-check"></i>
                      <h6 class="text-white">VIEW CART</h6>
                    </a>
                  </div>
                </div>
              </div>
              <h6 class="text-black">{{element.text}}</h6>
              <h6>{{element.price}}</h6>
            </div>
          </div>
        </div>
      </div>
  </main>
</template>

<script>
export default {
    name : 'IndexMain',
    data: function(){
      return{
        product: [
          {
            image: "product-9-500x500.jpg",
            name: 'Bed (1)'
          },
          {
            image: "product-3-500x500.jpg",
            name: 'Food (6)'
          },
          {
            image: "product-2-500x500.jpg",
            name: 'Toys (6)'
          },
          {
            image: "product-4-500x500.jpg",
            name: 'Transport (6)'
          },
        ],
        food: [
          {
            name: 'Kibble',
            type: 'Dry dog food',
            image: "food-transparent-18.png",
            shop: 'Shop dry food'
          },
          {
            name: 'Moist',
            type: 'Canned dog food',
            image: "food-transparent-17.png",
            shop: 'Shop moist food'
          },
          {
            name: 'Frozen',
            type: 'Freeze-Dried dog food',
            image: "food-transparent-16.png",
            shop: 'Shop frozen food'
          }
        ],
        product2: [
          {
            image: "product-21-800x800.jpg",
            name: 'Transport cage',
            price: '$25.00'
          },
          {
            image: "product-20-800x800.jpg",
            name: 'Dog leash',
            price: '$25.00'
          },
          {
            image: "product-16-800x800.jpg",
            name: 'Animal transport cage',
            price: '$̶3̶5̶.̶0̶0̶ $25.00'
          },
          {
            image: "product-21-800x800.jpg",
            name: 'Colorful cat leash',
            price: '$12.00'
          }
        ],
        articles: [
          {
            image: "blog-1.jpg",
            overText: "How to loose leash walk your dog",
            text: 'How to loose leash walk your dog',
            date: 'April 21st, 2020'
          },
          {
            image: "blog-2.jpg",
            overText: "Stop cats from scratching furniture",
            text: 'Stop cats from scratching furniture',
            date: 'April 19st, 2020'
          },
          {
            image: "blog-3.jpg",
            overText: "Where to buy the best pet food",
            text: 'Where to buy the best pet food',
            date: 'April 18st, 2020'
          },
          {
            image: "blog-4.jpg",
            overText: "Proper care for your pet toys",
            text: 'Proper care for your pet toys',
            date: 'April 17st, 2020'
          }
        ],
        articles2: [
          {
            image: "product-4-500x500.jpg",
            text: 'Animal transport bag',
            price: '$29.00'
          },
          {
            image: "product-5-500x500.jpg",
            text: 'Animal transport cage',
            price: '$35.00'
          },
          {
            image: "product-10-500x500.jpg",
            text: 'Animal transport bag',
            price: '$29.00'
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";
p{
  padding: 0px 400px;
}

.item-card{
  width: 300px;
  height: 300px;
  background-color: $cards-color;
  transition: 1.3s;
  cursor: pointer;
  img{
    width: 100%;
  }
  &:hover{
      box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.50), 0 6px 20px 0 rgba(0, 0, 0, 1);
      transform: translateY(-20px);
  }
}

.my-container{
  margin: 0 auto;
  display: flex;
  padding: 0px 18%;
  gap: 1%;
  .food-card{
  width: 33%;
  height: 650px;
  background-image: url('../assets/images/bg-transparent-3.png');
  background-size: 300px;
  background-color: $color-brand;
  transition: 1.3s;
  cursor: pointer;
    h1{
      color: white;
    }
    h6{
      color: #43764a;
    }
    img{
      width: 289px;
      margin: 37px;
    }
    button{
      background-color: #3d6f42;
      padding: 8px 20px;
      border-radius: 50px;
      color: white;
    }
    &:hover{
      box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.50), 0 6px 20px 0 rgba(0, 0, 0, 1);
      transform: translateY(-20px);
    }
  }
}

.arrivals-weekly{
  margin: 0 auto;
  margin-top: 100px;
  width: 65%;
  height: 490px;
  background-image: url('../assets/images/banner-3-2x-scaled.jpg');
  background-size: cover;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: 1.2s;
  button{
    padding: 5px 20px;
    border-radius: 50px;
    color: black;
    background-color: white;
    &:hover{
        background-color: #3d6f42;
        color: white;
    }
  }
  &:hover{
      box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.50), 0 6px 20px 0 rgba(0, 0, 0, 1);
      transform: translateY(-20px);
  }
}

.my-row{
  margin: 0 auto;
  width: 68%;
  h6{
    color: #3d6f42;
  }
  button{
    padding: 5px 20px;
    border-radius: 50px;
    color: white;
    background-color: #3d6f42;
  }
}

#users-testimonials{
width: 100%;
height: 580px;
background-image: url('../assets/images/bg-transparent-3.png');
background-size: 300px;
background-color: $color-brand;
margin-top: 116px;
  p{
    font-size: 0.90em;
  }
  h6{
    color: #5f838a;
  }
}

#form{
  margin: 0 auto;
  width: 65%;
  height: 450px;
  margin-top: 120px;
  background-image: url('../assets/images/banner-7-2x-scaled.jpg');
  background-size: cover;
  padding: 102px 612px 70px 90px;
  input{
    background-color: #f8f5f2;
    border-radius: 50px;
    width: 350px;
    padding: 10px;
  }
  button{
    padding: 5px 40px;
    border-radius: 50px;
    color: white;
    background-color: #3d6f42;
  }
}

button{
  background-color: #3d6f42;
  padding: 5px 20px;
  border-radius: 50px;
  color: white;
}

#section-of-best-products{
  width: 100%;
  height: 820px;
  background-image: url('../assets/images/bg-transparent-3.png');
  background-color: $color-brand;
  margin-top: 80px;
  button{
    padding: 5px 20px;
    border-radius: 50px;
    color: black;
    background-color: white;
    &:hover{
        background-color: #3d6f42;
        color: white;
    }
  }
  #left-image{
    width: 50%;
    height: 480px;
    background-image: url('../assets/images/banner-8-2x.jpg');
    background-size: cover;
    transition: 1.2s;
    &:hover{
      box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.50), 0 6px 20px 0 rgba(0, 0, 0, 1);
      transform: translateY(-20px);
    }
  }
  #right-image{
    width: 50%;
    height: 480px;
    background-image: url('../assets/images/banner-9-2x.jpg');
    background-size: cover;
    transition: 1.2s;
    &:hover{
      box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.50), 0 6px 20px 0 rgba(0, 0, 0, 1);
      transform: translateY(-20px);
    }
  }
}

.item-card-2{
  width: 300px;
  height: 351px;
  background-color: #faf4f4;
  transition: 1.2s;
  cursor: pointer;
  &:hover{
      box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.50), 0 6px 20px 0 rgba(0, 0, 0, 1);
      transform: translateY(-20px);
  }
}

#special{
  background-color: green;
  width: 70px;
  margin: 10px;
  padding: 5px 18px;
  font-size: 0.90em;
  color: white;
  cursor: pointer;
}

.container-overlay{
  position: relative;
  width: 100%;
  .image{
    display: block;
    width: 100%;
    height: auto;
  }
  .icon{
    color: white;
    font-size: 30px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    text-align: center;
    .fa-check:hover {
      color: black;
    }
    background-color: rgba(0, 0, 0, 0.5);
    border-radius: 70px;
    padding: 20px;
  }
  .overlay{
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
    width: 100%;
    opacity: 0;
    transition: .3s ease;
    background-color: rgba(0, 0, 0, 0.2);
    h6:hover{
      color: black;
    }
  }
}

.container-overlay:hover .overlay {
  opacity: 1;
}

/*Librerie*/

.animate__fadeInDown{
    --animate-delay: 1.5s;
    --animate-duration: 3s;
}

.animate__bounceInUp{
  --animate-delay: 1.5s;
  --animate-duration: 3s;
}
</style>