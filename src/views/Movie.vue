<template>
  <div class="movie-page">
    <Navbar />
    <div class="container">
      <div class="single-movie mt-5">
        <div class="title mb-5">Movie title</div>
        <div class="movie-image mb-5">
          <div class="year mb-3">Year</div>
          <img src="../assets/2.png" alt="Movie-Image" class="image-fluid">
        </div>
        <p class="description">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eaque doloribus dolor itaque in totam laborum modi maxime assumenda eum quisquam, aperiam ipsum ipsam temporibus molestiae provident hic, distinctio eos odit.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from "@/components/AppNavbar.vue";
export default {
  components: {
    Navbar
  }
};
</script>

<style scoped lang="scss">
.movie-page {
  .title,
  .year,
  p.description {
    color: white;
  }
}
</style>