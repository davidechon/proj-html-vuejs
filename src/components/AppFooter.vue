<template>
 <footer>
  <div id="footerTop">
    <div class="container d-flex flex-row justify-content-between align-items-center">
      <div class="card-group">
        <div class="card card-bv">
          <img src="../assets/svgs/svg-7.svg" alt="logo" class="logo-small">
          <div class="card-body">
            <ul class="fs-6">
              <li>
              A Functional HTML Template for Corporate &amp; Business.
            </li>
            <li>
                <i class="fa-solid fa-phone icons"></i>
                +1(305)1234-5678
              </li>
              <li>
                <i class="fa-solid fa-envelope icons"></i>
                hello@example.com
              </li>
              <li>
                <i class="fa-solid fa-location-dot icons"></i>
                Main Avenue, 987
              </li>
            </ul>
            <button class="btn btn-outline-cta" type="button">Get In Touch</button>
          </div>
        </div>
        <div class="card">
          <div class="card-body card-body-dark">
            <h2 class="title">About</h2>
              <ul class="listLink">
                <li v-for=" (item, index) in about" :key="index" >
                  <span class="listPoint">&rsaquo; </span> {{item.text}}
                </li>
              </ul>  
          </div> <!-- /card-body about-->
        </div> <!-- /card about -->
        <div class="card">
          <div class="card-body card-body-dark">
            <h2 class="title">Services</h2>
              <ul class="listLink">
                <li v-for="(item, index) in services" :key="index" >
                  <span class="listPoint">&rsaquo; </span> {{item.text}}
                </li>
              </ul>  
          </div> <!-- /card-body services -->
        </div> <!-- /card services -->
        <div class="card">
          <div class="card-body card-body-dark">
            <h2 class="title">Support</h2>
              <ul class="listLink">
                <li v-for="(item, index) in support" :key="index" >
                  <span class="listPoint">&rsaquo; </span> {{item.text}}
                </li>
              </ul>  
          </div> <!-- /card-body support -->
        </div> <!-- /card support -->
      </div> <!-- /card-group -->
    </div> <!-- /container cards-footer -->
  </div> <!-- /footerTop-->

  <div id="footerBottom">
    <div class="container d-flex justify-content-between align-items-center">
      <div>Enjoy the low price. We are tracking any intention of piracy</div>
      <div>&copy; 2020 NEXGEN is Proudly Powered by <span class="text-evidence">Codings</span>.</div>
      <span class="btn-outline-cta-rounded">
        <a href="#parallax"><i class="fa-solid fa-circle-arrow-up"></i></a>
      </span>
    </div> <!-- /container -->
  </div> <!-- /footerBottom-->
 </footer>
</template>

<script>

export default {
  name: 'AppFooter',
  data(){
    return{
      about:[
            {  
              "category": "about",
              "text": "The Company"
            },
            {  
              "category": "about",
              "text": "Institutional"
            },
            {  
              "category": "about",
              "text": "Social & Events"
            },
            {  
              "category": "about",
              "text": "Innovation"
            },
            {  
              "category": "about",
              "text": "Environment"
            },
            {  
              "category": "about",
              "text": "Technology"
            },
        ],
      services:[
        {  
          "category": "service",
          "text": "Audit & Assurance"
        },
        {  
          "category": "service",
          "text": "Financial Advision"
        },
        {  
          "category": "service",
          "text": "Analytics M&A"
        },
        {  
          "category": "service",
          "text": "Middle Marketing"
        },
        {  
          "category": "service",
          "text": "Legal Consulting"
        },
        {  
          "category": "service",
          "text": "Regulatory Risk"
        },
      ],
      support:[
        {  
          "category": "support",
          "text": "Responsibility"
        },
        {  
          "category": "support",
          "text": "Terms of Use"
        },
        {  
          "category": "support",
          "text": "About Cookies"
        },
        {  
          "category": "support",
          "text": "Privacy Polici"
        },
        {  
          "category": "support",
          "text": "Accessibility"
        },
        {  
          "category": "support",
          "text": "Information"
        }
      ]

    }
  }
}
</script>

<style lang='scss'>
@import '../styles/variables.scss';

footer{
  // height: 90vh;
  background: #121217;


  #footerTop{
    
    .container{
      background: #121217;
      height: 630px;
      position: relative;
    }
    .card-group{
      height: 330px;
      width: 100%;
      margin: 0 auto;
    }
    .card{
      color: #bcbebc;
      background: transparent;
      padding: auto 50px;
      margin: 10px;
      min-width: 250px;
    }
    
    .card-body-dark{
      background: #18181d;
      border: 1px solid #18181d;
      border-radius: 15px;
    }
    .card-body ul{
      width: 230px;
      padding-left: 0;
      list-style-type: none;
      font-size: 1.2rem;
    }
    .listPoint{
      font-size: 1.8rem;
    }
    .card-body ul li{
      font-size: 1.2rem;
      margin: 3px 0 5px;
      // padding: 0;
      line-height: 30px;
    }
    
    h2 .title{
      color: #ffffff;
      font-weight: 900;
    }

    .logo-small{
      width: 200px;
    }

      .btn-outline-cta{
      color: $text-color-light;
      border:1px solid $btn-cta-dark;
      padding: 10px 20px;
      margin: 10px 20px;
      font-size: 1.2rem;
      }

  } // /footerTop

  #footerBottom{
    color: #bcbebc;
    background: #121217;
    height: 80px;


     .text-evidence{
    color: $text-color-evidence;
    }

    .btn-outline-cta-rounded{
    color: $btn-cta-dark;
    padding: 0;
    margin: 10px 20px;
    font-size: 2rem;
    border-radius: 50%;
    overflow: hidden;
    }
    .btn-outline-cta-rounded a{
    color: $btn-cta-dark;
    }

  } // /footerBottom

} // /Footer

</style>