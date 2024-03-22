
<script>
import mainProduct from './partials/mainProduct.vue';
import db from "../db.json";
import { computed } from 'vue';
  export default {
    data(){
      return{
        db
        
      }

    },
    components:{
      mainProduct
    },



  }
</script>

<template>
  <main>
    <mainProduct 
      v-for="(item, index) in db.products"
      :key="index"
      :urlImg = "item.frontImage"
    />
  </main>
</template>


<style lang="scss" scoped>

@use "../assets/scss/partials/variables" as *;

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

.product .cuore:hover{
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