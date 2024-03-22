<script>
  export default {
    data(){
     return{
     priceD: 0
    } 
  },

  methods:{
      discountPrice(price, discount){
        this.priceD = (price * discount)/ 100;
      }
  },
    props:{
      
        urlImg: String,
        urlImg2: String,
        brand: String,
        nameProduct: String,
        priceProduct: Number,
        productData: Object
      
  },

  mounted(){
    
  }

    
}
</script>

<template>
  
    <div class="product">
      <img class="foto1" :src="'src/assets/img/'+urlImg" alt="">
      <img :src="'src/assets/img/'+urlImg2" alt="1b">
      <p>{{ brand }}</p>
      <h3>{{nameProduct}}</h3>
      <span class="prezzo">{{priceProduct}} &euro;</span>
      <div  class="badges">
        <span :class="productData.isInFavorites === true ? 'red' : '' " class="cuore d-flex ">&hearts;</span>
        <span v-for="(i, indice) in productData.badges" :key="indice" v-show="i.type === 'discount'" class="discount d-flex">{{ i.value }}</span>
        <span v-for="(i, indice) in productData.badges" :key="indice" v-show="i.type === 'tag'" class="eco d-flex">{{ i.value }}</span>
        
      </div>
    </div>
  
</template>


<style lang="scss" scoped>
@use "../../assets/scss/partials/variables" as *;
@use "../../assets/scss/partials/general" as *;

.container{
  flex-wrap: wrap;
}

.container .product{
  margin: 40px auto;
}

.product{
  position: relative;
  display: inline-block;

}

.product img{
  cursor: pointer;
  width: 465px;
  height: 670px;
}

.product .cuore{
  position: absolute;
  top: 0;
  right: 0;
  align-items: center;
  justify-content: center;
  background-color: $color-white;
  height: 50px;
  width: 50px;
  margin-top: 10px;
  font-size: 2rem;
}

.red{
  color: $color-prezzo;
}

.product .discount{
  position: absolute;
  bottom: 0;
  left: 0;
  align-items: center;
  justify-content: center;
  text-align: center;
  background-color: $color-white;
  width: 55px;
  height: 25px;
  margin-bottom: 100px;
  background-color: $color-prezzo;
  color: $color-white;
}

.product .eco{
  position: absolute;
  bottom: 0;
  left: 0;
  align-items: center;
  justify-content: center;
  text-align: center;
  background-color: $color-white;
  width: 100px;
  height: 25px;
  margin-bottom: 100px;
  margin-left: 60px;
  background-color: green;
  color: $color-white;
}


.product .eco-last{
  position: absolute;
  bottom: 0;
  left: 0;
  align-items: center;
  justify-content: center;
  text-align: center;
  background-color: $color-white;
  width: 100px;
  height: 25px;
  margin-bottom: 100px;
  background-color: green;
  color: $color-white;
}

.prezzo{
  color: $color-prezzo;
  font-weight: 800;
}

.line-through{
  text-decoration: line-through;
}

.product .foto1{
  position: absolute;
  top: 0;
  left: 0;
}

.product:hover .foto1{
  display: none;
}
</style>