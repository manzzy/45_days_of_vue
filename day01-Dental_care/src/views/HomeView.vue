<template>
  <div>
    <!-- Structure 
            1. Header
            2. Hero Section
            3. Ratings Section 
            4. Benefits Section
            5. Services Section
            6. Testimonials Section
            7. Footer
        -->
    <div class="wrapper">
      <HeaderComponent />
      <HeroComponent />
    </div>

    <RatingsComponent />
  </div>
</template>

<script setup>
    import HeaderComponent from '../components/HeaderComponent.vue'
    import HeroComponent from '../components/HeroComponent.vue'
    import RatingsComponent from '../components/RatingsComponent.vue'
</script>

<style scoped>
    @import url('../assets/styles/home.css');
</style>
