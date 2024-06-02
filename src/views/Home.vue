<!-- src/views/Home.vue -->
<template>
  <div>
    <Header />
    <Body />
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import Body from "../components/Body.vue";
import Footer from "../components/Footer.vue";

export default {
  name: "Home",
  components: {
    Header,
    Body,
    Footer,
  },
};
</script>

<style scoped>
/* CSS dành riêng cho view này nếu cần */
</style>
