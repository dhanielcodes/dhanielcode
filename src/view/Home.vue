<template>
  <div class="home">
    <div>
      <div class="en">
        <h3>Daniel Adekoya</h3>
      </div>
      <div class="en">
        <h1 class="h1h">
          I’m a Frontend Engineer <br />
          and UI Developer
        </h1>
      </div>
      <div class="en">
        <p class="p">
          I help build scalable frontend applications with<br />
          proper design system given to me
        </p>
      </div>

      <div class="img">
        <img src="../assets/face.svg" alt="" />
      </div>
      <p class="scroll">Scroll</p>
    </div>
  </div>
</template>

<script>
import { onMounted } from "vue";
import gsap from "gsap";
export default {
  setup() {
    onMounted(() => {
      gsap.from("h3, .h1h, .p", 1, {
        transform: "translateY(300%)",
        ease: "expo",
        delay: 2,
      });
      gsap.from(".img", 1, {
        transform: "translateY(20%)",
        /* transform: "translateY(300%)", */
        opacity: 0,
        ease: "expo",
        delay: 2.2,
      });
      gsap.from(".scroll", 1, {
        transform: "translateY(20%) translateX(-50%)",
        /* transform: "translateY(300%)", */
        opacity: 0,
        ease: "expo",
        delay: 2.6,
      });
    });

    return {};
  },
};
</script>

<style scoped>
.scroll {
  position: absolute;
  bottom: 40px;
  left: 50%;
  transform: translateX(-50%) translateY(0%);
}
.home {
  position: relative;
  text-align: center;
  min-height: 100vh;
  display: grid;
  place-items: center;
  padding: 10px;
}
h3,
h1,
p {
  margin-bottom: 20px;
}
h3 {
  font-weight: 300;
}
h1 {
  font-weight: 400;
}
p {
  color: #b1b1b1;
  font-weight: 300;
}
.img {
  padding: 20px;
  display: grid;
  place-items: center;
  width: 150px;
  background: #5a5a5a;
  height: 150px;
  margin: auto;
  border-radius: 50%;
}
.img img {
  width: 100%;
}
</style>
