<template>
 <section id="app">
<div class="header">
   <!-- {{datiInput[3].label}} -->
   <app-header/>
</div>
 
  <div class="main ">
    <app-main/>
  </div>
 
   <!-- <div class="footer debug">FOOTER
     <app-footer />
   </div> -->

 </section>
    

</template>

<script>
// import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import dati from './dati.json'
export default {
  name: 'App',
  components: { AppHeader, AppMain,
  //  AppFooter 
   },
  data(){
    return{
      datiInput: dati
    }
  }
   

}
</script>

<style lang="scss">
@import './styles/generals.scss';
@import './styles/variables.scss';


</style>