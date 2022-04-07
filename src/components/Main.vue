<template>
  <div>
    <div class="container-fluid text-center p-5">
      <div class="row p-5">
        <div class="col-12">
          <h2>Browse by category</h2>
          <p class="fs-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Fugit, atque inventore odio, ipsa numquam possimus earum blanditiis illo sed reprehenderit libero eligendi consequuntur eum quidem non aspernatur et, molestias quos.</p>
        </div>
      </div>
    </div>
    <div class="container-fluid">
      <div class="row justify-content-center mb-5">
        <div class="col-2 text-center mb-5" v-for="(element, index) in product" :key="'primo'+index">
          <div class="item-card">
            <img :src="require(`../assets/images/${element.image}`)" alt="">
          </div>
          <h5 class="mt-4">{{element.name}}</h5>
        </div>
      </div>
    </div>
      <!---->
    <div class="my-container">
      <div class="food-card d-flex flex-column text-center align-items-center justify-content-center" v-for="(element, index) in food" 
      :key="'secondo'+index">
        <h1>{{element.name}}</h1>
        <h6>{{element.type}}</h6>
        <img :src="require(`../assets/images/${element.image}`)"  alt="">
        <button class="border-0">{{element.shop}}</button>
      </div>
    </div>
    <div class="arrivals-weekly">
      <h6 class="text-white mb-4">FIND THE BEST ANIMAL SUPPLIES</h6>
      <h2 class="text-white fs-1 fw-bolder mb-4">New arrivals weekly</h2>
      <button class="border-0 text-black">Learn more about us</button>
    </div>
    <div class="section-best-sellers">
      
    </div>
  </div>
</template>

<script>
export default {
    name : 'IndexMain',
    data: function(){
      return{
        product: [
          {
            image: "product-9-300x300.jpg",
            name: 'Bed (1)'
          },
          {
            image: "product-3-300x300.jpg",
            name: 'Food (6)'
          },
          {
            image: "product-2-300x300.jpg",
            name: 'Toys (6)'
          },
          {
            image: "product-4-300x300.jpg",
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
            name: 'Kibble',
            type: 'Dry dog food',
            image: "food-transparent-17.png",
            shop: 'Shop moist food'
          },
          {
            name: 'Kibble',
            type: 'Dry dog food',
            image: "food-transparent-16.png",
            shop: 'Shop frozen food'
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
}

.my-container{
  margin: 0 auto;
  display: flex;
  width: 1250px;
  gap: 1%;
  .food-card{
  width: 33%;
  height: 490px;
  background-image: url('../assets/images/bg-transparent-3.png');
  background-size: 300px;
  background-color: $color-brand;
    h1{
      color: white;
    }
    h6{
      color: #43764a;
    }
    img{
      width: 200px;
    }
    button{
      background-color: #3d6f42;
      padding: 5px 20px;
      border-radius: 50px;
      color: white;
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
  button{
    padding: 5px 20px;
    border-radius: 50px;
    color: white;
  }
}
</style>