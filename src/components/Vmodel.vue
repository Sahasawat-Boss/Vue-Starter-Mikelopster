<!-- - ผูก State ตัวแปลเข้ากับ Html Tag -->
<script setup>
import { ref } from "vue";

const searchText = ref("");
</script>

<template>
  <div>
    <h2>V-Model Comps Test</h2>
    <div>Search:{{ searchText }}</div>
    <input v-model="searchText" />
  </div>
</template>
