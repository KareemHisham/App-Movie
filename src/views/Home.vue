<template>
  <div id="home">
    <Navbar />
    <Header />
    <Form />
  </div>
</template>

<script>
  import Navbar from "@/components/AppNavbar.vue";
  import Header from "@/components/app-header.vue";
  import Form from "@/components/App-Form.vue";

export default {
  components: {
    Navbar,
    Header,
    Form
  }
};
</script>
