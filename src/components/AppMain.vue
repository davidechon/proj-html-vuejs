<template>
  <main>
    <div id="parallax">
      <div class="container-fluid">
        <div class="container">
          <div class="row d-flex justify-content-center align-items-center text-box">
            <div class="col-8 text-center">
              <h1>Ready  <span class="text-evidence">Team</span></h1>
              <h4 class="col-7">No matter what your company needs, we will be ready to assist you in the best possible way.</h4>
              <button class="btn btn-cta" type="button">Get in Touch</button>
             <button class="btn btn-outline-cta" type="button">Read more</button>
            </div> <!-- /parallax container col-6 -->
           </div> <!-- /parallax container row -->
        </div> <!-- /parallax container -->
      </div> <!-- /parallax container-fluid -->

    </div> <!-- /parallax -->


    <div id="service" class="debug">Service
        <div class="container debug">
          <div class="row debug">
            <h4>Our business areas</h4>
            <h2>Excellence in <span class="text-evidence">Services</span></h2>
            <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of expedienced and renowned professionals. These are some options that you can hire</p>
            <button class="btn btn-cta" type="button">See all</button>
          </div> <!-- /service - container - row -->

          <div class="row">
            <ul>
              <li>
                <img src="../assets/svgs/svg-1.svg" alt="svg-1" class="icons">
                <i class="fa-solid fa-arror-right icons"></i>
                <h3>Audit & Assurance</h3>
                <p>Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </li>
              <li>
                <img src="../assets/svgs/svg-2.svg" alt="svg-2" class="icons">
                <i class="fa-solid fa-arror-right icons"></i>
                <h3>Financial Advisory</h3>
                <p>Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </li>
               <li>
                <img src="../assets/svgs/svg-3.svg" alt="svg-3" class="icons">
                <i class="fa-solid fa-arror-right icons"></i>
                <h3>Analytics and Advisory</h3>
                <p>Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </li>
               <li>
                <img src="../assets/svgs/svg-4.svg" alt="svg-4" class="icons">
                <i class="fa-solid fa-arror-right icons"></i>
                <h3>Middle Marketing</h3>
                <p>Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </li>
               <li>
                <img src="../assets/svgs/svg-5.svg" alt="svg-5" class="icons">
                <i class="fa-solid fa-arror-right icons"></i>
                <h3>Legasl consulting</h3>
                <p>Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </li>
               <li>
                <img src="../assets/svgs/svg-6.svg" alt="svg-5" class="icons">
                <i class="fa-solid fa-arror-right icons"></i>
                <h3>Regulaory risk</h3>
                <p>Lorem ipsum dolor sit amet consecteur adipiscing elit.</p>
              </li>
            </ul>
          </div> <!-- /service - container - row - cards-->
        </div> <!-- /service - container -->
    </div> <!-- /service -->


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

<style lang='scss' scope>
@import '../styles/variables.scss';

main{

  #parallax{
    background-image: url(../assets/img/bg-parallax.png);
    background-position: top;
    height: 90vh;
    margin-top: 10px;
    border: 1px solid red;
    // background: 
    //       linear-gradient(
    //           to left,
    //           transparent 0px,
    //           transparent 20px,
    //           rgba(#000, 0.02) 20px,
    //           rgba(#000, 0.02) 40px
    //       ),
    //       linear-gradient(
    //           to bottom,
    //           transparent 0px,
    //           transparent 20px,
    //           rgba(#000, 0.02) 20px,
    //           rgba(#000, 0.02) 40px
    //       );
    //       background-size: 40px, 100% 40px;
          

    .container{
      margin-top: 380px;
    
      h1{
        font-size: 4rem;
        font-weight: 900;
      }
      h4{
        margin: 10px auto;
        font-size: 1.2rem;
        font-weight: 300;
        color: $text-color-middle;
      }
      

      .text-box{
        height: 300px;
        margin: 20px auto;
        font-size: 2rem;
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

    } // /parallax container

  } // /#parallax

} // /main

#service{
  height: 90vh;
  margin-top: 10px;


  .icons{
    width: 50px;
    height: 50px;
    color: #007f87;
    font-size: 12px;
    border: 1px solid green;
  }
  .fa-solid .fa-arror-right{
    // width: 50px;
    // height: 50px;
    color: #007f87;
    font-size: 18px;
    border: 1px solid green;
  }
} // /main - service

</style>