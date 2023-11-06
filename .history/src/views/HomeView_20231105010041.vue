<template>
  <div class="home">
    <img src="../assets/mf-avatar.svg" alt="happy person" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "HomeView",
  components: {
    HelloWorld,
  },
};
</script>
<style scoped>
img {
  margin-bottom: 20px;
}
</style>
