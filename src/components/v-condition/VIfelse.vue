<script setup>
import { ref } from 'vue'

const awesome = ref(true)

</script>

<template>
  <div>
    <button @click="awesome = !awesome">Toggle</button>

    <h1 v-if="awesome">สวัสดี</h1>
    <h1 v-else>ไม่นะ 😢</h1>
  </div>
</template>