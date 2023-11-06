<template>
  <div class="home">
    <img
      src="../assets/WhatsApp_Image_2023-11-05_at_12.44.03_AM-removebg-preview.png"
      alt="Personal Photo"
      height="300px"
    />
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
