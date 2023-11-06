<template>
  <div>
    <component :is="component"></component>
    <div class="view">
      <a :href="link" target="_blank">Preview Project</a>
      <div class="control">
        <button type="button" @click="goBack">
          <span>&larr;</span>
          Previous Project
        </button>
        <button type="button" @click="controlComponent">
          Next Project <span>&rarr;</span>
        </button>
      </div>
    </div>
  </div>
</template>
<style scoped>
.view {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
button,
a {
  background-color: #261c33;
  margin-top: 1rem;
  padding: 10px 20px;
  color: white;
  box-shadow: 1px 1px 5px 1px white;
  border-radius: 20px;
  cursor: pointer;
  text-decoration: none;
  transition: all 0.5s;
  /* font-weight: bold; */
  font-size: 1.5rem;
}
button:hover {
  transform: translateX(10px);
}
a:hover {
  transform: translateY(5px);
}
span {
  margin: 10px;
}
.control {
  display: flex;
  gap: 10rem;
}
</style>

<script>
import CRUD from "../components/TheCRUD.vue";
import Bankist from "../components/TheBankist.vue";
import Weather from "../components/TheWeather.vue";
import Battleground from "../components/TheBattleground.vue";
import Rock from "../components/RockPaper.vue"
export default {
  components: { CRUD, Bankist, Weather, Battleground ,Rock},
  data() {
    return {
      counter: 0,
      component: "CRUD",
      link: "https://ahamdy997.github.io/CRUDS-System/",
    };
  },
  methods: {
    controlComponent() {
      if(this.counter>4)return;
      this.counter++;
    },
    goBack() {
      if(this.counter<0)return;
      this.counter--;
    },
  },
  watch: {
    counter() {
      if (this.counter === 0) {
        this.component = "CRUD";
        this.link = "https://ahamdy997.github.io/CRUDS-System/";
      } else if (this.counter === 1) {
        this.component = "Bankist";
        this.link = "https://ahamdy997.github.io/Bankist/";
      } else if (this.counter === 2) {
        this.component = "Weather";
        this.link = "https://ahamdy997.github.io/WeatherApp/";
      } else if (this.counter === 3) {
        this.component = "Battleground";
        this.link = "https://ahamdy997.github.io/VueBattleGround/";
      }else if (this.counter === 4) {
        this.component = "Rock";
        this.link = "https://ahamdy997.github.io/RockPaperScissor/";
    }
  },
};
</script>
