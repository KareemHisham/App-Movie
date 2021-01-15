<template>
  <div id="home">
    <Navbar />
    <Header />
    <Form />
    <Movies />
  </div>
</template>

<script>
import Navbar from "@/components/AppNavbar.vue";
import Header from "@/components/app-header.vue";
import Form from "@/components/App-Form.vue";
import Movies from "@/components/App-Movies.vue";

export default {
  components: {
    Navbar,
    Header,
    Form,
    Movies
  }
};
</script>
