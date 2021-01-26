<template>
  <div class="projects">
    <div>
      <div class="head">
        <h1>Assets</h1>
        <img src="../assets/element.svg" alt="" />
      </div>
      <div class="works">
        <div class="work" v-for="(item, idx) in works" :key="idx">
          <div class="work_lang">
            <div class="work_lang_tag" v-for="(lan, idx) in item.lang" :key="idx">
              {{ lan.name }}
            </div>
          </div>

          <div class="work_desc">
            <h2>{{ item.title }}</h2>
            <p>{{ item.desc }}</p>
          </div>

          <a :href="item.link" target="_blank">
            <img src="../assets/link.svg" alt="" />
          </a>
        </div>
      </div>
      <a href="https://github.com/dhanielcodes" target="_blank">
        <button>
          <span>Github for more</span> <img src="../assets/link.svg" alt="" />
        </button>
      </a>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const works = ref([
      {
        lang: [{ name: "Vue" }, { name: "CSS" }],
        title: "Boton",
        desc: "A simple CSS library for getting nice styled custom buttons",
        link: "https://boton.vercel.app/",
      },
      {
        lang: [{ name: "Vue" }],
        title: "Github Users",
        desc: "Type in a github username to see his or her stats",
        link: "https://getgithubuser.vercel.app/",
      },
      {
        lang: [{ name: "Vue" }],
        title: "Unsplash Clone",
        desc: "A clone of the unsplash image website",
        link: "https://unsplash-clone.vercel.app/",
      },
      {
        lang: [{ name: "Vue" }, { name: "Vite" }],
        title: "Vitejs State Management Template",
        desc:
          "A simple state management clone, with vue's vite js. Can be used to manage small vue apps with less data or medium",
        link: "https://github.com/dhanielcodes/vite-state-management-template",
      },
      {
        lang: [{ name: "Vue" }, { name: "GraphQL" }, { name: "Apollo" }],
        title: "Block - Q",
        desc:
          "I used the bitquery API to get data of different crypto coins, information data and displayed them",
        link: "https://block-q.vercel.app/",
      },
      {
        lang: [{ name: "Vue" }, { name: "Rest API" }, { name: "JWT" }],
        title: "Tudu",
        desc: "Tudu is an activity manager web app",
        link: "https://tudu-olive.vercel.app/",
      },
    ]);

    return { works };
  },
};
</script>

<style scoped>
.projects {
  min-height: 100vh;
  display: grid;
  place-items: center;
  padding: 40px 0px;
}
.projects .head {
  text-align: center;
}
.works {
  margin-top: 50px;
  display: grid;
  grid-template-columns: repeat(3, 300px);
  grid-template-rows: repeat(2, 300px);
  grid-gap: 10px;
}
.works .work {
  background: #0000004d;
  padding: 25px;
  border-radius: 10px;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-direction: column;
}
.work .work_lang {
  display: flex;
  justify-content: space-between;
}
.work_lang .work_lang_tag {
  padding: 4px 7px;
  border-radius: 6px;
  background: #41414152;
  margin-right: 6px;
}
.work h2 {
  font-size: 15px;
  margin-bottom: 10px;
}
.work p {
  font-size: 13px;
  font-weight: 200;
}
button {
  padding: 15px 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #0000004d;
  color: white;
  border: none;
  border-radius: 8px;
  margin-top: 20px;
  outline: none;
  cursor: pointer;
}
a {
  text-decoration: none;
}
button span {
  margin-right: 10px;
  font-size: 16px;
}
@media (max-width: 1080px) {
  .works {
    margin-top: 50px;
    display: grid;
    padding: 0 20px;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(3, 300px);
    grid-gap: 10px;
  }
}
@media (max-width: 710px) {
  .works {
    margin-top: 50px;
    display: grid;
    padding: 0 20px;
    grid-template-columns: repeat(1, 1fr);
    grid-template-rows: repeat(6, 300px);
    grid-gap: 10px;
  }
}
</style>
