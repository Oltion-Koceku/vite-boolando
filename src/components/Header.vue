<script>
  export default {
  }
</script>

<template>
  
  <header>
    <div class="topbar">
      <div class="container d-flex box">
        <!-- nav -->
        <nav class="menu d-flex">
          <ul class="d-flex">
            <li>
              <a href="#">Donna</a>
            </li>
            <li>
              <a href="#">Uomo</a>
            </li>
            <li>
              <a href="#">Bambini</a>
            </li>
          </ul>
        </nav>
        <!-- /nav -->

        <!-- logo -->
        <div class="logo">
          <img src="../assets/img/boolean-logo.png" alt="logo">
        </div>
        <!-- /logo -->

        <!-- icon -->
        <nav class="menu social">
          <ul class="d-flex">
            <li>
              <a href="#"><i class="fa-regular fa-user"></i></a>
            </li>
            <li>
              <a href="#"><i class="fa-regular fa-heart"></i></a>
            </li>
            <li>
              <a href="#"><i class="fa-solid fa-bag-shopping"></i></a>
            </li>
          </ul>
        </nav>
        <!-- /icon -->

      </div>
    </div>
  </header>
  
</template>


<style lang="scss" scoped>
@use "../assets/scss/partials/variables";
header{
  margin: 0 auto;
  .topbar{
    background-color: #FF6900;
    width: 100%;
    height: 60px;
    position: fixed;
    z-index: 1;
    top: 0;
    left: 0;

    .box{
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 100%;
      margin: 0 17%;

      .menu ul{
        display: flex;
        list-style: none;
        justify-content: space-between;

        a{
          color: white;
          text-decoration: none;
          margin-right: 10px;

          &:hover{
            text-decoration: underline;
          }
        }
      }

      .logo{
        width: 300px;
        img{
          max-width: 30%;
        }
      }
    }
  
  }
}

</style>