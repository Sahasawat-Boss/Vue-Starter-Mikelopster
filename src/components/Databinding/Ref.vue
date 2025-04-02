<script setup>
import { ref } from 'vue' //Concept Ref

defineProps({
  msg: String,
})

const counter = ref(0) //store ref 0 >> when Update >> change html 

const increase =() =>{
  counter.value = counter.value + 1
}
</script>

<template>
  <div>
  <div>Hello Comps</div>
  <div>Couter {{ counter }}</div>
  <button @click="increase">Add Couter</button>
  </div>

</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
