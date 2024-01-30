<template>
  
    <div id="carousel" class="carousel slide" data-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active" data-target="#carousel" data-slide-to="0" >
      <div> <PageAbout/> </div>
    </div>
    <div class="carousel-item" data-target="#carousel" data-slide-to="1">
      <div> <PageStudies/> </div>
    </div>
    <div class="carousel-item" data-target="#carousel" data-slide-to="2">
      <div> <PageProjects/> </div>
    </div>
    <div class="carousel-item" data-target="#carousel" data-slide-to="3">
      <div> <PageContact/> </div>
    </div>
  </div>
  <!--<button class="carousel-control-prev" type="button" data-bs-target="#carousel" data-bs-slide="prev">
    <span class="carousel-control-prev-icon visually-hidden" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carousel" data-bs-slide="next">
    <span class="carousel-control-next-icon visually-hidden" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>-->
</div>
</template>

<script setup>
import PageAbout from './PageAbout.vue';
import PageStudies from './PageStudies.vue';
import PageProjects from './PageProjects.vue';
import PageContact from './PageContact.vue';

</script>


<style scoped>

.carousel{
  border:none;
}


</style>