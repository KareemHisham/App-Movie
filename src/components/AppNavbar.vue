<template>
  <nav>
    <router-link to="/" class="nav">
      <h1>
        <span>Vue</span>
        Movie
      </h1>
    </router-link>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      title: "Vue"
    };
  }
};
</script>

<style scoped lang="scss">
nav {
  background: #264653;
  padding: 15px;
  .nav {
    justify-content: center;
    align-items: center;
    text-decoration: none;
    h1 {
      color: white;
      span {
        color: #42b983;
      }
    }
  }
}
</style>
