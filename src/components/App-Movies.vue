<template>
  <div id="movies">
    <div class="container">
      <div class="movies">
        <div class="item">
          <div class="movie-img">
            <img src="../assets/2.png" alt="Movie-Name" />
            <span>Series</span>
          </div>
          <div class="movie-details">
            <div class="year">1990</div>
            <h3 class="title">Movie Name</h3>
          </div>
        </div>
        <div class="item">
          <div class="movie-img">
            <img src="../assets/2.png" alt="Movie-Name" />
            <span>Series</span>
          </div>
          <div class="movie-details">
            <div class="year">1990</div>
            <h3 class="title">Movie Name</h3>
          </div>
        </div>
        <div class="item">
          <div class="movie-img">
            <img src="../assets/2.png" alt="Movie-Name" />
            <span>Series</span>
          </div>
          <div class="movie-details">
            <div class="year">1990</div>
            <h3 class="title">Movie Name</h3>
          </div>
        </div>
        <div class="item">
          <div class="movie-img">
            <img src="../assets/2.png" alt="Movie-Name" />
            <span>Series</span>
          </div>
          <div class="movie-details">
            <div class="year">1990</div>
            <h3 class="title">Movie Name</h3>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
#movies {
  margin-top: 30px;
  .movies {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    .item {
      flex-basis: 48%;
      margin-bottom: 15px;
      .movie-img {
        position: relative;
        img {
          width: 100%;
        }
        span {
          position: absolute;
          left: 0;
          bottom: 20px;
          background-color: #42b983;
          color: white;
          border-radius: 0px 7px 7px 0;
          padding: 3px 10px;
          font-size: 20px;
        }
      }
    }
  }
}
</style>
