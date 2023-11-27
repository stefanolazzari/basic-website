<script setup>
import HeaderComponent from './components/HeaderComponent.vue'
// import FooterComponent from './components/HeaderComponent.vue'
import HeaderComponentcopy from './components/HeaderComponentcopy.vue'

</script>


<template>
  <div
    :class="[
      {
        'bg-01': this.$route.name == 'Home',
        'bg-02': this.$route.name == 'About',
        'bg-03': this.$route.name == 'Cv',
        'bg-04': this.$route.name == 'Projects',
        'bg-05': this.$route.name == 'Metodo',
        'bg-06': this.$route.name == 'Contatti'
      }
    ]"
  >
    <header>
      
    </header>

    <body>
      <HeaderComponent></HeaderComponent>
      <router-view />
    </body>

    <!-- <footer>
      <Footer-component></Footer-component>
    </footer> -->
  </div>
</template>

<style scoped>
</style>
