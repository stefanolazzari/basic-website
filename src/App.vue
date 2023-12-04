<script setup>
import HeaderComponent from './components/HeaderComponent.vue'
// import FooterComponent from './components/HeaderComponent.vue'



document.cookie = 'valore=7800 ; name=stefano; expires=' + new Date(2024,0,1).toUTCString();
//document.cookie = 'valore=7800';
console.log(document.cookie);


</script>


<template>
  <div class="bg-image-01">
    <header>
      
    </header>

    <body>
      <HeaderComponent></HeaderComponent>
      <router-view class="p-10"></router-view>
    </body>

    <!-- <footer>
      <Footer-component></Footer-component>
    </footer> -->
  </div>
</template>

<style scoped>



</style>
