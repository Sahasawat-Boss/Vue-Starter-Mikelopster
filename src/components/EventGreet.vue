<script setup>
import { ref } from "vue"; // Import ref
const name = ref("Vue.js");

const greet = (event) => {
  console.log("event", event);
  alert(`Hello ${name.value}!`);
  // `event` is the native DOM event
  if (event) {
    alert(event.target.tagName);
  }
};
</script>

<template>
  <button @click="greet">Greet</button>
</template>
