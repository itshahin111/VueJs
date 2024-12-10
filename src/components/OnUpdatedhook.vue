<template>
  <div>
    <h1>Hooks</h1>
  </div>
  <h1>{{ message }}</h1>
  <button @click="message = 'Hello From Ostad'">Update Message</button>
  <HelloWorld msg="Vite + Vue" />
</template>

<script setup>
import { ref, onUpdated } from "vue";
import HelloWorld from "./components/HelloWorld.vue";
const message = ref("Hello World!");
onUpdated(() => {
  console.log("App.vue updated!");
});
</script>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
