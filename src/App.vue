<template>
  <div class="container-fluid m-0 p-0">

    <div class="container-fluid nav-bar m-0 p-0">
      <NavBar/>
    </div>

    <div class="container-fluid m-0 p-0 carousel">
      <CarouselContainer/> 
    </div>

    <div class="container-fluid m-0 p-0 footer">
      <FooterBar/>

    </div>

  </div>
  
</template>

<script setup>
import NavBar from './components/NavBar.vue';
import FooterBar from './components/FooterBar.vue';
import CarouselContainer from './components/CarouselContainer.vue';

</script>

<style scoped>

body{
  margin: 0;
  padding: 0;
  background-color:#28292A;
}

</style>
