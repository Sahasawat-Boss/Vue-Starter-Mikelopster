<script setup>
import Reactive from './components/Databinding/Reactive.vue';
</script>

<template>
  <main class="Main">
    <h2 class="Head">Main</h2>
    <Reactive />
  </main>
</template>

<style scoped>
.Main{
  padding: 15px;
  color: rgba(255, 255, 255, 0.87);
  background-color: #242424;
  height: fit-content;
}

.Head{
  color: aquamarine;
}

</style>
