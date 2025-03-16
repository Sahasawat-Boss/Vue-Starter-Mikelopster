<script setup>
import { ref } from "vue";

const searchText = ref("");
</script>

<template>
  <h2>V-Model Comps Test</h2>
  <input v-model="searchText" />
  <br>
  <div>{{ searchText }}</div>
</template>
