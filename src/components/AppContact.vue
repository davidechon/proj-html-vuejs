<template>
  <section id="contact" class="contact">
      <div class="container">
        <div class="row">
          <div class="col-6">
            <div class="row g-2">

              <div>
                <h4 class="text-evidence">send a message</h4>
                <h2>Get in <span class="text-evidence">Touch</span></h2>
                <p>We will respond to your message as soon as possible.</p>
              </div> <!-- /contact title text -->

              <div class="formInput d-flex flex-wrap justify-content-center align-items-center">
                <div class="col-md">
                <input id="name" type="text" class="form-control"  placeholder="Name" aria-label="Name">
                <input id="phone" type="text" class="form-control"  placeholder="Phone" aria-label="phone">
              </div>
              <div class="col-md">
                <input id="floatingInputGrid" type="email" class="col-6 form-control" placeholder="Email">
                <div class="col-md">
                  <select class="form-select" id="moreInfo" aria-label="Floating label select example">
                    <option>More Info</option>
                    <option value="1">One</option>
                    <option value="2">Two</option>
                    <option value="3">Three</option>
                  </select>
                </div>
              </div>
              <div class="col-12">
                <textarea class="form-control" id="exampleFormControlTextarea1" rows="5" placeholder="Message"></textarea>
              </div>
              </div>

              <div class="col-12">
                <button class="btn btn-cta" type="submit">Send</button>
              </div>


            </div> <!-- /form -->

          </div>  <!-- /col-6 form-->
          <div class="col-6">
            <h3>Example Inc.</h3>
            <p class="text-start">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            <p class="text-start">Praesent diam lacus, dapibus sed imperdiet consectetur.</p>
            <div class="row d-flex flex-wrap justify-content-center align-items-center">
              <div class="listIcons">
              <i class="fa-solid fa-phone btn-outline-cta-rounded"></i>
              <h5>+1(305)1234-5678</h5>
            </div>
            <div class="listIcons">
              <i class="fa-solid fa-envelope btn-outline-cta-rounded"></i>
              <h5>hello@example.com</h5>
            </div>
            <div class="listIcons">
              <i class="fa-solid fa-location-dot btn-outline-cta-rounded"></i>
             <h5> Main Avenue, 987</h5>
            </div>
            </div>
            <button class="btn btn-outline-cta" type="button">View Map</button>
          </div>  <!-- /col-6 view map-->
        </div> <!-- /row -->
      </div>  <!-- /container -->

    </section> <!-- /contact -->
</template>

<script>
export default {
  name: 'AppContact',
}
</script>


<style lang='scss'>
@import '../styles/variables.scss';

#contact{
  margin-top: 100px;
  margin-bottom: 100px;

    h2{
      margin-top: 30px;
      margin-bottom: 30px;
      font-weight: 600;
      font-size: 2rem;
    }

   h2 .text-evidence{
    background-color: $bg-color-evidence;
    color: $text-color-evidence;
    font-weight: 900;
    padding: 10px;
    border-radius: 5px;
  }
  h4 .text-evidence{
    color: #0e272d;
    padding: 10px;
  }


 h3{
   padding-left: 18px;
   color: $text-color-dark;
   font-weight: 500;
 }
 p.text-start{
   padding-left: 20px;
   color: $text-color-dark;
   font-weight: 200;
 }
 
 h5{
   margin: 20px;
   color: $btn-cta-dark;
   font-weight: 200;
 }
 .listIcons{
   display: inline-flex;
   padding: 10px 20px;
 }
 .btn-cta{
      background: $btn-cta-dark;
      color: $text-color-light;
      padding: 10px 20px;
      font-size: 1.2rem;
      }

 .btn-outline-cta{
      color: $btn-cta-dark;
      border:1px solid $btn-cta-dark;
      padding: 10px 20px;
      margin: 10px 20px;
      font-size: 1.2rem;
      }

  .btn-outline-cta-rounded{
    background: $bg-color-evidence;
    color: $btn-cta-dark;
    padding: 0.7rem;
    margin: 10px;
    font-size: 1.5rem;
    border-radius: 50%;
    overflow: hidden;
    }




// Form style
.formInput{
  padding: 10px 0;
}
 .form-control, .form-select{
   background-color: $bg-middle;
   color: $text-color-middle;
   border: 0;
   border-radius: 5px;
   margin: 15px 0 10px;
 }
 .form-select{
   color: $text-color-dark;
 }












} // /#contact
</style>