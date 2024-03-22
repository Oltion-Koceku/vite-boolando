<script>
  export default {
    props(){
      return{
        urlImg: String,
        urlImg2: String,
        brand: Number,
        nameProduct: String,
        priceProduct: String
      }
    },

    mounted(){
      console.log(this.brand);
    }

    
  }
</script>

<template>
  <div class="container d-flex ">
    <div class="product">
      <img class="foto1" src="../../assets/img/{{ urlImg }}" alt="">
      <img src="../assets/img/{{urlImg2}}" alt="1b">
        <span class="cuore d-flex ">&hearts;</span>
        <span class="discount d-flex">-50%</span>
        <span class="eco d-flex">Sostenibilitá</span>
        <p>{{ brand }}</p>
        <h3>{{nameProduct}}</h3>
        <span class="prezzo">{{priceProduct}} &euro;</span>
        <span class="overline line-through">29,99 &euro;</span>
    </div>
  </div>
</template>


<style lang="scss" scoped>

</style>