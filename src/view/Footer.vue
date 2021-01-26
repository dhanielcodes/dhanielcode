<template>
  <div class="footer">
    <footer>
      <div class="en">
        <h1 class="footh">Get in touch !</h1>
      </div>
      <div class="line"></div>
      <div class="en">
        <div class="mail">
          <a href="mailto:adekoyadaniel53@gmail.com" target="_blank"
            >adekoyadaniel53@gmail.com</a
          >
        </div>
      </div>
      <div class="socials">
        <a href="https://twitter.com/daniel_adekoya_">
          <img src="../assets/twitter.svg" alt="" />
        </a>
        <a href="https://www.linkedin.com/in/daniel-adekoya-010810192/">
          <img src="../assets/linkedin.svg" alt="" />
        </a>
        <a href="https://github.com/dhanielcodes/">
          <img src="../assets/github.svg" alt="" />
        </a>
      </div>
    </footer>
  </div>
</template>

<script>
import { onMounted } from "vue";
import gsap from "gsap";
export default {
  setup() {
    onMounted(() => {
      gsap.from(".footh, .mail", 1, {
        transform: "translateY(300%)",
        ease: "expo",
        scrollTrigger: {
          trigger: ".footer",
          toggleActions: "restart",
          start: "top center",
        },
      });
      gsap.from(".socials", 1, {
        transform: "translateY(20%)",
        /* transform: "translateY(300%)", */
        opacity: 0,
        ease: "expo",
        scrollTrigger: {
          trigger: ".footer",
          toggleActions: "restart",
          start: "top center",
        },
        delay: 0.2,
      });
    });

    return {};
  },
};
</script>

<style scoped>
.footer {
  text-align: center;
  min-height: 100vh;
  display: grid;
  place-items: center;
  padding: 10px;
}
h1 {
  font-weight: 300;
  font-size: 40px;
}
.line {
  width: 500px;
  height: 1px;
  background: white;
  margin: 30px 0;
}
.socials {
  margin-top: 30px;
}
.socials img {
  margin: 0 10px;
}
@media (max-width: 580px) {
  .line {
    width: 100%;
  }
  .socials img {
  }
}
</style>
