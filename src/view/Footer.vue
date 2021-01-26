<template>
  <div class="footer">
    <footer>
      <h1>Get int touch !</h1>
      <div class="line"></div>
      <a class="mail" href="mailto:adekoyadaniel53@gmail.com" target="_blank"
        >adekoyadaniel53@gmail.com</a
      >
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
export default {};
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
