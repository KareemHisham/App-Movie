<template>
  <div id="header">
    <div class="main-movie-card">
      <router-link to="/movie">
        <img src="../assets/2.png" alt="movie" />
        <div class="main-movie-description">
          <h3 class="title">Prince Of Persia</h3>
          <p class="decription">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Saepe
            laboriosam tempora dignissimos mollitia, excepturi corrupti velit
            natus qui numquam molestiae magnam. Tempora cupiditate ab iure. Est
            laborum unde porro magnam!
          </p>
        </div>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
#header {
  position: relative;
  a {
    text-decoration: none;
    img {
      width: 100%;
      height: 80vh;
    }
    .main-movie-description {
      position: absolute;
      bottom: 0;
      background-color: rgba($color: #000000, $alpha: 0.6);
      padding: 15px;
      .title,
      .decription {
        color: white;
      }
      .title {
        color: #42b983;
      }
    }
  }
}
</style>
