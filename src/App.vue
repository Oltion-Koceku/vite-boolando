
<script>
  import Footer from './components/Footer.vue';
  import Header from './components/Header.vue';
  import Main from './components/Main.vue';
  import {json} from './data/db.js'
  
  
  export default {
    data(){
      return{
        json
        
      }
    },
    components:{
      
      Header,
      Main,
      Footer,
    }    
  }
</script>

<template>

  <Header />
  <Main />
  <Footer />

</template>


<style lang="scss">
  @use "./assets/scss/main.scss"
</style>