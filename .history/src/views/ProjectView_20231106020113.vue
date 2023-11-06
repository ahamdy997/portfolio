<template>
  <div>
    <component :is="component"></component>
    <div class="view">
      <a href="https://ahamdy997.github.io/CRUDS-System/" target="_blank"
        >Review Project</a
      >
      <div class="control">
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
  margin-top: 1.5rem;
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
  margin-left: 10px;
}
</style>

<script>
import CRUD from "../components/TheCRUD.vue";
import Bankist from "../components/TheWeather.vue";
export default {
  components: { CRUD, Bankist },
  data() {
    return {
      counter: 0,
      component: "CRUD",
    };
  },
  methods: {
    controlComponent() {
      this.counter++;
      if (this.counter === 1) {
        this.component = "Bankist";
      }
    },
  },
};
</script>
