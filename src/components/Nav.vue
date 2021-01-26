<template>
  <div class="nav">
    <div class="circle" @click="open = !open">
      <svg
        :class="{ open: open }"
        width="32"
        height="32"
        viewBox="0 0 32 32"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <rect
          x="17.9199"
          width="32"
          height="3.84"
          rx="1.92"
          transform="rotate(90 17.9199 0)"
          fill="white"
        />
        <rect
          x="32"
          y="17.92"
          width="32"
          height="3.84"
          rx="1.92"
          transform="rotate(-180 32 17.92)"
          fill="white"
        />
      </svg>
    </div>
    <ul :class="{ open: open }">
      <li><a href="">About</a></li>
      <li><a href="">Reach out</a></li>
      <li><a href="">Works</a></li>
    </ul>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const open = ref(false);

    return { open };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.nav {
  position: fixed;
  top: 0;
  left: 50%;
  transform: translateX(-50%) translateY(-12%);
}
.circle {
  width: 100px;
  height: 100px;
  display: grid;
  place-items: center;
  border-radius: 50%;
  background: #65656527;
  backdrop-filter: blur(10px);
  margin: auto;
  padding: 20px;
  cursor: pointer;
}
.circle svg {
  transform: translateY(55%) rotate(0);
  transition: all 0.3s;
}
.circle svg.open {
  transform: translateY(55%) rotate(45deg);
}
ul {
  padding: 20px 40px;
  list-style: none;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-direction: column;
  background: #65656527;
  width: 300px;
  margin: 10px 0;
  border-radius: 10px;
  backdrop-filter: blur(10px);
  opacity: 0;
  pointer-events: none;
  transform: translateY(-10px);
  transition: all 0.3s;
}
ul.open {
  transform: translateY(0px);
  pointer-events: all;
  opacity: 1;
}
ul li {
  margin: 20px 0;
}
ul li a {
  text-decoration: none;
}
</style>
