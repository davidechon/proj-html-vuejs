<template>
  <header class="container-fluid">
    <div id="headerTop" class="container">
      <div class="row">
        <div class="d-flex justify-content-between align-items-center">
          <span class="d-flex justify-content-start align-items-center">
            <i class="fa-solid fa-clock"> Open Hours: Mon - Sat - 9:00 - 18:00</i>
          </span>
          <span class="d-flex justify-content-end align-items-center">
            <i class="fa-solid fa-phone"> +1(305)1234-5678</i> 
            <i class="fa-solid fa-envelope"> hello@example.com</i>
            <i class="fa-brands fa-facebook-f"></i>
            <i class="fa-brands fa-twitter"></i>
            <i class="fa-brands fa-linkedin-in"></i>
          </span>
        </div> <!-- /headerTop row span -->
      </div> <!-- /headerTop row -->
    </div> <!-- /headerTop container -->

    <div id="headerBottom" class="container">
      <div class="row">
        <div class="d-flex justify-content-between align-items-center">
          <span class="d-flex justify-content-start align-items-center">
            <img class="logo" src="../assets/logo.png" alt="logo">
          </span>
          
          <ul class="d-flex justify-content-end align-items-center">
            <!-- <li><a href="#parallax">HOME</a></li>
            <li><a href="#service">SERVICE</a></li>
            <li><a href="#about">ABOUT</a></li>
            <li><a href="#projects">PROJECTS</a></li>
            <li><a href="#results">RESULTS</a></li>
            <li class="btn btn-cta"><a href="#contact">GET IN TOUCH</a></li> -->
            <li>HOME</li>
            <li>SERVICE</li>
            <li>ABOUT</li>
            <li>PROJECTS</li>
            <li>RESULTS</li>
            <li class="btn btn-cta">GET IN TOUCH</li>
          </ul>
        </div> <!-- /headerBottom row div -->
      </div> <!-- /headerBottom row -->
    </div> <!-- /headerBottom -->
  </header>
</template>

<script>
export default {
  name: 'AppHeader',
}
</script>

<style lang='scss' scope>
@import '../styles/variables.scss';

header{
  // position: fixed;
  top:0;
  left:0;
  width: 100%;
  z-index: 1;
  height: 70px;
  background: $bg-dark;
  // margin-bottom: 100px;

  // a{
  //   text-decoration: none;
  //   color: #bcbebc;
  // }
  // a:hover{
  //   cursor: pointer;
  // }

  #headerTop{
    height: 70px; 
    line-height: 70px;
    background: $bg-dark;
    color: $text-color-light;

    .fa-solid{
      margin: 15px;
      padding: 10px;
      color: $bg-middle;
      font-size: 0.7rem;
      font-weight: 200;
      letter-spacing: 0.1rem;
      text-transform: capitalize;
    }
    .fa-brands{
      margin: 0 15px;
    }


  } // /HeaderTop 

  #headerBottom{
    height: 70px; 
    line-height: 70px;
    background: $bg-light;
    color: $text-color-dark;
    position: relative;

    .logo {
    position: absolute;
    top: 15px;
    left: 20px;
    width: 120px;
    }
    
    ul li{
      list-style-type: none;
      margin: auto 20px;
      font-size: 1.1rem;
      font-weight: 700;
    }
    .btn-cta{
      background: $btn-cta-dark;
      color: $text-color-light;
      padding: 10px 20px;
    }

  } // /HeaderBottom

} // /Header 



</style>