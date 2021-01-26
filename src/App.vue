<template>
  <Home />
  <About />
  <Projects />
  <Footer />
</template>

<script>
import Home from "./view/Home.vue";
import About from "./view/About.vue";
import Projects from "./view/Projects.vue";
import Footer from "./view/Footer.vue";

export default {
  name: "App",
  components: {
    Home,
    About,
    Projects,
    Footer,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800&display=swap");
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
}
</style>
