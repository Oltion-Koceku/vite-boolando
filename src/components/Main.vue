
<script>
  export default {
    
  }
</script>

<template>
  <main>
    <div class="container d-flex ">
      
      <!-- Top items -->
      <div class="product">
        <img class="foto1" src="../assets/img/1.webp" alt="">
        <img src="../assets/img/1b.webp" alt="1b">
          <span class="cuore d-flex ">&hearts;</span>
          <span class="discount d-flex">-50%</span>
          <span class="eco d-flex">Sostenibilitá</span>
          <p>Levi's</p>
          <h3>RELAXED FIT TEE UNISEX</h3>
          <span class="prezzo">14,99 &euro;</span>
          <span class="overline line-through">29,99 &euro;</span>
      </div>

      <div class="product">
          <img class="foto1" src="../assets/img/2.webp" alt="">
          <img src="../assets/img/2b.webp" alt="2b">
          <span class="cuore d-flex ">&hearts;</span>
          <span class="discount  d-flex">-30%</span>
          <p>Guess</p>
          <h3>ROSES TEE</h3>
          <span class="prezzo">20,99 &euro;</span>
          <span class="overline line-through">29,99 &euro;</span>
        </div>  
        
        <div class="product">
          <img class="foto1" src="../assets/img/3.webp" alt="">
          <img src="../assets/img/3b.webp" alt="3b">
          <span class="cuore d-flex ">&hearts;</span>
          <span class="discount d-flex">-30%</span>
          <p>Come zucchero filato</p>
          <h3>VOGLIA DI COLORI PASTELLO</h3>
          <span class="prezzo">129,99 &euro;</span>
          <spa class="overline line-through">184,99 &euro;</spa>
        </div>
          <!-- /Top items -->

          <!-- Bottom items -->
          <div class="product">
            <img class="foto1" src="../assets/img/4.webp" alt="">
            <img src="../assets/img/4b.webp" alt="4b">
            <span class="cuore d-flex ">&hearts;</span>
            <span class="discount d-flex">-50%</span>
            <span class="eco d-flex">Sostenibilitá</span>
            <p>Levi's</p>
            <h3>TEE UNISEX</h3>
            <span class="prezzo">14,99 &euro;</span>
            <span class="overline line-through">29,99 &euro;</span>
          </div>
          
          <div class="product ">
            <img class="foto1" src="../assets/img/5.webp" alt="">
            <img src="../assets/img/5b.webp" alt="5b">
            <span class="cuore d-flex ">&hearts;</span>
            <span class="discount d-flex">-50%</span>
            <span class="eco d-flex">Sostenibilitá</span>
            <p>Maya Deluxe</p>
            <h3>STRIPE BODICE</h3>
            <span class="prezzo">99,99 &euro;</span>
          </div>
          
          <div class="product">
            <img class="foto1" src="../assets/img/6.webp" alt="">
            <img src="../assets/img/6b.webp" alt="6b">
            <span class="cuore d-flex ">&hearts;</span>
            <span class="eco-last d-flex">Sostenibilitá</span>
            <p>Esprit</p>
            <h3>MAGLIONE - BLACK</h3>
            <span class="prezzo">29,99 &euro;</span>
          </div>

    </div>
</main>
</template>


<style lang="scss" scoped>

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
  background-color: white;
  height: 50px;
  width: 50px;
  margin-top: 10px;
  font-size: 2rem;
}

.product .cuore:hover{
  color: red;
}

.product .discount{
  position: absolute;
  bottom: 0;
  left: 0;
  align-items: center;
  justify-content: center;
  text-align: center;
  background-color: white;
  width: 55px;
  height: 25px;
  margin-bottom: 100px;
  background-color: red;
  color: white;
}

.product .eco{
  position: absolute;
  bottom: 0;
  left: 0;
  align-items: center;
  justify-content: center;
  text-align: center;
  background-color: white;
  width: 100px;
  height: 25px;
  margin-bottom: 100px;
  margin-left: 60px;
  background-color: green;
  color: white;
}


.product .eco-last{
  position: absolute;
  bottom: 0;
  left: 0;
  align-items: center;
  justify-content: center;
  text-align: center;
  background-color: white;
  width: 100px;
  height: 25px;
  margin-bottom: 100px;
  background-color: green;
  color: white;
}

.prezzo{
  color: red;
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