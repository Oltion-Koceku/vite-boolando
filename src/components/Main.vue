
<script>
import mainProduct from "./partials/mainProduct.vue";
import {json} from "../data/db.js"


  export default {
    data(){
      return{
        jsonlist : json
        
      }

    },
    components:{
      mainProduct
    },

    mounted(){
      console.log();
    }



  }
</script>

<template>
  <main>
    <div class="container d-flex ">
      <mainProduct 
        v-for="(item, index) in jsonlist.products"
        :key="index"
        :urlImg = "item.frontImage"
        :brand = "item.brand"
        :urlImg2 = "item.backImage"
        :nameProduct = "item.name"
        :priceProduct = "item.price"
        :productData="item"
        
      />
    </div>
  </main>
</template>


<style lang="scss">



</style>