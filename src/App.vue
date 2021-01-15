<template>
  <div id="app">
      <home />
      <movie />
  </div>
</template>

<script>
import Home from '@/views/Home.vue';
import Movie from '@/views/Movie.vue';
  export default {
    components: {
      Home,
      Movie
    }
}
</script>

<style lang="scss">
 * {
   margin: 0;
   padding: 0;
   box-sizing: border-box;
 }
 body {
   background-color: #1d3557 !important;
 }
</style>