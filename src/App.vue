<template>
 <section id="app">
<div class="header">
   <app-header/>
</div>
 
  <div class="main ">
    <app-main/>
  </div>
 
  <div class="footer">
    <app-footer />
  </div>

 </section>
    

</template>

<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';

export default {
  name: 'App',
  components: { AppHeader, AppMain, AppFooter 
   },
  // data(){
  //   return{
      
  //   }
  // }
   

}
</script>

<style lang="scss">
@import './styles/generals.scss';
@import './styles/variables.scss';


</style>