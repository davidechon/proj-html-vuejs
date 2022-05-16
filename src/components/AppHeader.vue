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
  height: 70px;
  background: $bg-dark;
  margin-bottom: 100px;

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