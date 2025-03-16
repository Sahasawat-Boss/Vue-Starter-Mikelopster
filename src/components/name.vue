<script setup>
import { ref } from 'vue'
const name = ref('')

const onInput = (event) => {
  name.value = event.target.value
}
</script>
<template>
  <div>
    <input type="text" :value="name" @input="onInput">
    <p>Hello, {{ name }}!</p>
  </div>
</template>