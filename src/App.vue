<template>
 <section>
<div class="header debug">HEADER
   <app-header/>
</div>
 
  <div class="main debug">MAIN
    <app-main/>
  </div>
 
   <div class="footer debug">FOOTER
     <app-footer />
   </div>

 </section>
    

</template>

<script>
import AppFooter from './components/AppFooter.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
export default {
  name: 'App',

  components: { AppHeader, AppMain, AppFooter },
   

}
</script>

<style lang="scss">
@import './styles/generals.scss';
@import './styles/variables.scss';


</style>