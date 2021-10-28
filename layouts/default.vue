<template>
  <div class="main-content">
    <Navigation />
    <Nuxt />
  </div>
</template>
<style>
body {
  background: #2d3436;
  color: white;
  font-family: Arial, Helvetica, sans-serif;
  padding: 20px;
}
</style>
<script>
import Navigation from '../components/Navigation.vue'
export default {
  components: {
    Navigation,
  },
}
</script>