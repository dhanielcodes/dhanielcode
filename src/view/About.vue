<template>
  <div class="about">
    <div>
      <p>
        Am a solution focused web developer with experience in web-based<br />
        applications. Participated in development and implementation of web based
        solutions,<br />
        while gaining real World experience. Learning multiple systems and efficient<br />
        development techniques
      </p>
      <div class="btns">
        <a
          href="https://docs.google.com/document/d/e/2PACX-1vQNIAyJ53JZSh9H5PWDktdG1RgDvtb_fSnE4v5Jt5KjvGssmpXqoAuknLIoveFSdSuBJVIkh4oM0FDe/pub"
          target="_blank"
        >
          <button><span>Resume</span> <img src="../assets/link.svg" alt="" /></button>
        </a>
        <a href="#work">
          <button><span>Works</span> <img src="../assets/link.svg" alt="" /></button>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.about {
  text-align: center;
  min-height: 100vh;
  display: grid;
  place-items: center;
  padding: 10px;
}
.about p {
  font-size: 20px;
  font-weight: 300;
}
.btns {
  margin-top: 30px;
  width: 100%;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
.btns button {
  padding: 15px 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #0000004d;
  color: white;
  border: none;
  border-radius: 8px;
  margin: 10px;
  outline: none;
  cursor: pointer;
  width: 150px;
}
.btns a {
  text-decoration: none;
}
.btns button span {
  margin-right: 10px;
  font-size: 16px;
}
</style>
