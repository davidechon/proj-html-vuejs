<template>
  <main>
    <section id="parallax">
      <div class="container-fluid">
        <div class="container container-parallax">
          <div class="row d-flex justify-content-center align-items-baseline">
            <div class="col col-8 text-center">
              <h1>Ready  <span class="text-evidence">Team</span></h1>
              <h4 class="col-7">No matter what your company needs, we will be ready to assist you in the best possible way.</h4>
              <button class="btn btn-cta" type="button">Get in Touch</button>
             <button class="btn btn-outline-cta" type="button">Read more</button>
            </div> <!-- /parallax container col-8 -->
           </div> <!-- /parallax container row -->
        </div> <!-- /parallax container -->
      </div> <!-- /parallax container-fluid -->

    </section> <!-- /parallax -->


    <section id="service">
        <div class="container">
          <div class="row">
            <h4 class="service">Our business areas</h4>
            <h2 class="service">Excellence in <span class="text-evidence">Services</span></h2>
            <p class="service">We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of expedienced and renowned professionals. These are some options that you can hire</p>
            <button class="btn btn-cta" type="button">See all</button>
          </div> <!-- /service - container - row -->

          <div class="row row-cols-3 gx-3">
            <div class="card mb-3">
              <div class="card-header d-flex justify-content-between">
                <img src="../assets/svgs/svg-1.svg" alt="svg-1" class="icons">
                <i class="fa-solid fa-arrow-right icons"></i>
              </div> <!-- /card header -->
              <div class="card-body">
                <h5 class="card-title">Audit & Assurance</h5>
                <p class="card-text">Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </div>
            </div> <!-- /card 1 -->
            <div class="card text-dark mb-3">
              <div class="card-header d-flex justify-content-between">
                <img src="../assets/svgs/svg-2.svg" alt="svg-1" class="icons">
                <i class="fa-solid fa-arrow-right icons"></i>
              </div> <!-- /card header -->
              <div class="card-body">
                <h5 class="card-title">Financial Advisory</h5>
                <p class="card-text">Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </div>
            </div> <!-- /card 2 -->
            <div class="card text-dark mb-3">
              <div class="card-header d-flex justify-content-between">
                <img src="../assets/svgs/svg-3.svg" alt="svg-1" class="icons">
                <i class="fa-solid fa-arrow-right icons"></i>
              </div> <!-- /card header -->
              <div class="card-body">
                <h5 class="card-title">Analytics and Advisory</h5>
                <p class="card-text">Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </div>
            </div> <!-- /card 3 -->

            <div class="card text-dark mb-3">
              <div class="card-header d-flex justify-content-between">
                <img src="../assets/svgs/svg-4.svg" alt="svg-1" class="icons">
                <i class="fa-solid fa-arrow-right icons"></i>
              </div> <!-- /card header -->
              <div class="card-body">
                <h5 class="card-title">Middle Marketing</h5>
                <p class="card-text">Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </div>
            </div> <!-- /card 4 -->
            <div class="card text-dark mb-3">
              <div class="card-header d-flex justify-content-between">
                <img src="../assets/svgs/svg-5.svg" alt="svg-1" class="icons">
                <i class="fa-solid fa-arrow-right icons"></i>
              </div> <!-- /card header -->
              <div class="card-body">
                <h5 class="card-title">Legal consulting</h5>
                <p class="card-text">Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </div>
            </div> <!-- /card 5 -->
            <div class="card text-dark mb-3">
              <div class="card-header d-flex justify-content-between">
                <img src="../assets/svgs/svg-6.svg" alt="svg-1" class="icons">
                <i class="fa-solid fa-arrow-right icons"></i>
              </div> <!-- /card header -->
              <div class="card-body">
                <h5 class="card-title">Regulatory Risk</h5>
                <p class="card-text">Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </div>
            </div> <!-- /card 6 -->
          </div> <!-- /row cards -->

        </div> <!-- /service - container -->
      </section> <!-- /service -->


    <div id="about" class="debug">Company</div>
    <div id="project" class="debug">Project</div>
    <div id="results" class="debug">Results</div>
    <div id="contact" class="debug">Contact</div>
  </main>
</template>

<script>
export default {
  name: 'AppMain',
}
</script>

<style lang='scss'>
@import '../styles/variables.scss';

main{

  #parallax .container-fluid{
    background-image: url(../assets/img/bg-parallax.png);
    background-position: center;
    background-origin: border-box;
    height: 90vh;
    position: relative;
    
    .container-parallax{
      position: relative;
      top: 30%;
      padding: 40px;

      .col h1{
        font-size: 4rem;
        font-weight: 900;
        padding: 10px;
      }
      .col h4{
        margin: 10px auto;
        font-size: 1.2rem;
        font-weight: 300;
        color: $text-color-middle;
      }
      
      
      
      .text-box{
        position: absolute;
        top: 10%;
        left: 20%;
        transform: translate();
        height: 300px;
        // margin: 20px auto;
        font-size: 2rem;
        border: 2px solid green;
      }

      .text-evidence{
        color: $text-color-evidence;
        background-color: $bg-color-evidence;
        padding: 10px;
      }

      .btn-cta{
      background: $btn-cta-dark;
      color: $text-color-light;
      padding: 10px 20px;
      font-size: 1.2rem;
      }
      .btn-outline-cta{
      background: $text-color-light;
      color: $btn-cta-dark;
      border:1px solid $btn-cta-dark;
      padding: 10px 20px;
      margin: 10px 20px;
      font-size: 1.2rem;
      }

   } // /#parallax container

  } // /#parallax



#service{
  height: 100vh;
  margin-top: 10px;
  background: #eef4ed;

  .service h2{
    // color: $text-color-evidence;
    font-size: 1.8rem;
    text-transform: uppercase;
    font-weight: 900;
    padding-top: 10px; 
    }
  .service h4{
    color: $text-color-evidence;
    font-size: 0.8rem;
    text-transform: uppercase;
    font-weight: 900;
    padding-top: 10px; 
    }

     .card{
      min-height: 300px;
      width: calc((100% / 3) - 60px);
      margin: 15px;
      padding: 20px;
      border-radius: 15px;
      background-color: #fff;
    }
    .card-header{}
    .card-body{}
    .card-title{}
    .card-text{}


  .icons{
    width: 50px;
    height: 50px;
    color: #007f87;
    font-size: 12px;
    border: 1px solid green;
  }
  .fas.fa-solid.fa-arrow-right{
    // width: 50px;
    // height: 50px;
    color: #007f87;
    font-size: 150px;
    border: 1px solid green;
  }




  } // /#service
   





} // /main

</style>