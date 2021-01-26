<template>
  <svg
    class="bg"
    width="1440"
    height="900"
    viewBox="0 0 1440 900"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <line
      y1="-1.5"
      x2="1673.76"
      y2="-1.5"
      transform="matrix(0.768019 0.640427 -0.429288 0.903168 -220.826 -108.124)"
      stroke="#404040"
      stroke-opacity="0.53"
      stroke-width="3"
    />
    <line
      y1="-1.5"
      x2="1673.76"
      y2="-1.5"
      transform="matrix(0.768019 0.640427 -0.429288 0.903168 -553 178.759)"
      stroke="#404040"
      stroke-opacity="0.53"
      stroke-width="3"
    />
    <line
      y1="-1.5"
      x2="1673.76"
      y2="-1.5"
      transform="matrix(0.768019 0.640427 -0.429288 0.903168 -405.383 8.74002)"
      stroke="#404040"
      stroke-opacity="0.53"
      stroke-width="3"
    />
    <line
      y1="-1.5"
      x2="1673.76"
      y2="-1.5"
      transform="matrix(0.768019 0.640427 -0.429288 0.903168 -16.4446 -183.381)"
      stroke="#404040"
      stroke-opacity="0.53"
      stroke-width="3"
    />
    <line
      y1="-1.5"
      x2="1673.76"
      y2="-1.5"
      transform="matrix(0.768019 0.640427 -0.429288 0.903168 236.43 -227.586)"
      stroke="#404040"
      stroke-opacity="0.53"
      stroke-width="3"
    />
    <line
      y1="-1.5"
      x2="1673.76"
      y2="-1.5"
      transform="matrix(0.768019 0.640427 -0.429288 0.903168 459.781 -290.493)"
      stroke="#404040"
      stroke-opacity="0.53"
      stroke-width="3"
    />
    <line
      y1="-1.5"
      x2="1673.76"
      y2="-1.5"
      transform="matrix(0.768019 0.640427 -0.429288 0.903168 707.52 -350)"
      stroke="#404040"
      stroke-opacity="0.53"
      stroke-width="3"
    />
  </svg>
  <Nav />
  <Home />
  <About id="about" />
  <Projects id="work" />
  <Footer id="reach" />
</template>

<script>
import Nav from "./components/Nav.vue";

import Home from "./view/Home.vue";
import About from "./view/About.vue";
import Projects from "./view/Projects.vue";
import Footer from "./view/Footer.vue";

export default {
  name: "App",
  components: {
    Nav,
    Home,
    About,
    Projects,
    Footer,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800&display=swap");
html,
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
  color: white;
}
body {
  min-height: 100vh;
  background: #2d2d2d;
}
.bg {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  z-index: -1;
}
.en {
  overflow: hidden;
}
</style>
