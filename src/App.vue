
<script>
  import Footer from './components/Footer.vue';
  import Header from './components/Header.vue';
  import Main from './components/Main.vue';
  
  export default {
    data(){
      return{
        Header,
        Main,
        Footer
      }
    }    
  }
</script>

<template>
  <Header />
  <Main />
  <Footer />

</template>


<style lang="scss">

</style>