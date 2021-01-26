<template>
  <div class="home">
    <div>
      <h3>Daniel Adekoya</h3>
      <h1>
        I’m a Frontend Engineer <br />
        and UI Developer
      </h1>
      <p>
        I help build scallable frontend applications with<br />
        proper design system given to me
      </p>
      <div class="img">
        <img src="../assets/face.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.home {
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
