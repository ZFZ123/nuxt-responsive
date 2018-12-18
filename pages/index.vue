<template>
  <div>
    <!--导航-->
    <div class="navbar-wrapper">
      <div class="container">
        <nav class="navbar navbar-inverse navbar-static-top">
          <div class="container">
            <div class="navbar-header">
              <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar">
                <span class="sr-only">Toggle navigation</span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
                <span class="icon-bar"></span>
              </button>
              <a class="navbar-brand" href="#">
                <Logo></Logo>
              </a>
            </div>
            <div id="navbar" class="navbar-collapse collapse">
              <ul class="nav navbar-nav">
                <li class="active"> <nuxt-link to="/">小牛</nuxt-link></li>
                <li> <nuxt-link to="/">商城</nuxt-link></li>
                <li> <nuxt-link to="/">体验店</nuxt-link></li>
                <li> <nuxt-link to="/">服务</nuxt-link></li>
                <li> <nuxt-link to="/">新闻</nuxt-link></li>
                <li> <nuxt-link to="/">骑行数据</nuxt-link></li>
                <li> <nuxt-link to="/">关于我们</nuxt-link></li>
              </ul>
            </div>
          </div>
        </nav>

      </div>
    </div>


    <div id="myCarousel" class="carousel slide" data-ride="carousel">
      <!-- Indicators -->
      <ol class="carousel-indicators">
        <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
        <li data-target="#myCarousel" data-slide-to="1"></li>
        <li data-target="#myCarousel" data-slide-to="2"></li>
      </ol>
      <div class="carousel-inner" role="listbox">
        <div class="item active">
          <div class="first-slide my-slide" >
            <img src="./../assets/img/max_img_1.jpg" alt="">

          </div>
          <div class="container">
            <div class="carousel-caption">
            </div>
          </div>
        </div>
        <div class="item">
          <div class="second-slide my-slide" >
            <img src="./../assets/img/max_img_2.jpg" alt="">

          </div>
          <div class="container">
            <div class="carousel-caption">
            </div>
          </div>
        </div>
        <div class="item">
          <div class="third-slide my-slide" >
            <img src="./../assets/img/max_img_3.jpg" alt="">
          </div>
          <div class="container">
            <div class="carousel-caption">
            </div>
          </div>
        </div>
      </div>
      <!--<a class="left carousel-control" href="#myCarousel" role="button" data-slide="prev">-->
        <!--<span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>-->
        <!--<span class="sr-only">Previous</span>-->
      <!--</a>-->
      <!--<a class="right carousel-control" href="#myCarousel" role="button" data-slide="next">-->
        <!--<span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>-->
        <!--<span class="sr-only">Next</span>-->
      <!--</a>-->
    </div><!-- /.carousel -->

    <div class="container marketing">

      <div class="row">
        <div class="col-lg-4">
          <img  src="./../assets/img/bottom_1.jpg" alt="Generic placeholder image" width="100%" height="100%">
          <h2>冬骑攻略</h2>
        </div><!-- /.col-lg-4 -->
        <div class="col-lg-4">
          <img   src="./../assets/img/bottom_2.jpg" alt="Generic placeholder image" width="100%" height="100%">
          <h2>新手行车指南</h2>
        </div><!-- /.col-lg-4 -->
        <div class="col-lg-4">
          <img   src="./../assets/img/bottom_3.jpg" alt="Generic placeholder image" width="100%" height="100%">
          <h2>官方智能APP</h2>
        </div><!-- /.col-lg-4 -->
      </div><!-- /.row -->

      <!-- FOOTER -->
      <footer>
        <p class="pull-right"><a href="#">顶部</a></p>
        <p>&copy; 2016 Company, Inc. &middot; <a href="#">小牛</a> &middot; <a href="#">团队</a></p>
      </footer>

    </div>

  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>

  body {
    padding-bottom: 40px;
    color: #5a5a5a;
  }


  /* 导航
  ------------------------ */

  .navbar-wrapper {
    position: absolute;
    top: 0;
    right: 0;
    left: 0;
    z-index: 20;
  }

  .navbar-wrapper > .container {
    padding-right: 0;
    padding-left: 0;
  }
  .navbar-wrapper .navbar {
    padding-right: 15px;
    padding-left: 15px;
  }
  .navbar-wrapper .navbar .container {
    width: auto;
  }

  .carousel {
    height: 100%;
  }
  .carousel-caption {
    z-index: 10;
  }
  .carousel .item {
    height: 100%;
    width: 100%;
    background-color: #777;
  }
  /*轮播图大小*/
  .carousel .item .my-slide{
    width: 100%;
    height: 100%;

  }
  .carousel .item .my-slide img{
    float: left;
  }
  .my-slide .img-info{
    width: 50%;
    height: 100%;
    background: rgba(0,0,0,0.5);
    z-index: 999999;
    position: absolute;
    right: 0;
  }
  .marketing{
    padding: 60px 40px;
    background: #333;
  }
  .marketing .col-lg-4 {
    margin-bottom: 20px;
    text-align: center;
  }
  .marketing h2 {
    position: absolute;
    margin: 10px auto;
    width: 100%;
    text-align: center;
    top:0;
    font-weight: normal;
  }
  .marketing .col-lg-4{
    padding: 0;
  }
  .marketing .col-lg-4 p {
    margin-right: 10px;
    margin-left: 10px;
  }




  /* media CSS
  -------------------------------------------------- */

  @media (min-width: 768px) {
    /* Navbar positioning foo */
    .navbar-wrapper {
      margin-top: 20px;
    }
    .navbar-wrapper .container {
      padding-right: 15px;
      padding-left: 15px;
    }
    .navbar-wrapper .navbar {
      padding-right: 0;
      padding-left: 0;
    }

    .navbar-wrapper .navbar {
      border-radius: 4px;
    }

    .carousel-caption p {
      margin-bottom: 20px;
      font-size: 21px;
      line-height: 1.4;
    }

    .my-slide img{
      height: 100%;
      width: 200%;
    }
  }
  @media (max-width: 768px) {
    .my-slide img{
      height: 100%;
      width: 200%;
    }
    .my-slide .img-info{
      display: none;
    }
  }
  @media (min-width: 992px) {
    .my-slide img{
      height: 100%;
      width: 100%;
    }
  }
  .container {
    width:100%
  }
</style>
