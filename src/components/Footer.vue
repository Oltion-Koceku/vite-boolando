
<script>
  export default {
    
  }
</script>

<template>
  <footer class="d-flex">
    <div class="container d-flex">
      <div>
        <h4>Boolando s.r.l</h4>
        <nav>
          <ul class="d-flex column">
            <li><a href="#">Infomazioni legali</a></li>
            <li><a href="#">Normativa sulla privacy</a></li>
            <li><a href="#">Diritto di recesso</a></li>
          </ul>
        </nav>
      </div>

      <div class="social">
        <h4>Trovaci anche su</h4>
        <a href=""><i class="fa-brands fa-x-twitter"></i></a>
        <a href=""><i class="fa-brands fa-square-facebook"></i></a>
        <a href=""><i class="fa-brands fa-instagram"></i></a>
        <a href=""><i class="fa-brands fa-pinterest"></i></a>
        <a href=""><i class="fa-brands fa-youtube"></i></a>
      </div>
    </div>
  </footer>
</template>


<style lang="scss" scoped>
footer{
  align-items: center;
  background-color: #1a1a1a;
  height: 100px;
  .container{
    justify-content: space-between;
    color: white;
    li{
      padding: 0;
      line-height: 40px;
      padding-right: 10px;
      a{
        text-decoration: none;
        color: white;
        margin-right: 10px;
      }
    }
    .social{
      a{
        color: white;
      }
    
      i{
      padding-right: 5px;
      font-size: large;
      line-height: 40px;
      }
    }
  }
}






</style>