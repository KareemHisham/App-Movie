<template>
  <div id="movies">
    <div class="container">
      <div class="movies">
        <router-link :to='"/movie/" + index' class="item text-decoration-none" v-for="(movie, index) in movies" :key="index">
          <div class="movie-img">
            <img :src="movie.Poster" alt="Movie-Name" />
            <span>{{movie.Type}}</span>
          </div>
          <div class="movie-details">
            <div class="year">{{movie.Year}}</div>
            <h3 class="title">{{movie.Title}}</h3>
          </div>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props:['movies']
};
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
      background: #14213d;
      border-radius: 0px 0 10px 10px;
      color: white;
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
      .movie-details {
        padding: 10px 0px 0px 10px;
      }
    }
  }
}
</style>
