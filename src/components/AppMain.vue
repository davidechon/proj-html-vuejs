<template>
  <main>
    <div id="jumbotron">

      <div class="container-fluid">
        <!-- <img src="../assets/img/bg-parallax.png" alt="jumbotron" class="col-12"> -->
        <div class="container">
          <div class="row d-flex justify-content-center align-items-center text-box">
            <div class="col-8 text-center">
              <h1>Ready  <span class="text-evidence">Team</span></h1>
              <h4 class="col-7">No matter what your company needs, we will be ready to assist you in the best possible way.</h4>
              <button class="btn btn-cta" type="button">Get in Touch</button>
             <button class="btn btn-outline-cta" type="button">Read more</button>
            </div> <!-- /Jumbotron container col-6 -->
         
            

           </div> <!-- /Jumbotron container row -->
        </div> <!-- /Jumbotron container -->
      </div> <!-- /Jumbotron container-fluid -->

    </div> <!-- /Jumbotron -->


    <div id="service" class="debug">Service</div>
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

  #jumbotron{
    background-image: url(../assets/img/bg-parallax.png);
    background-position: top;
    height: 90vh;
    margin-top: 10px;
    border: 1px solid green;
    

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


    } // /jumbotron container

  } // /#jumbotron

} // /main

</style>