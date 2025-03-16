<script setup>
//<<-- This show that what will it show first
import { reactive } from "vue";

const state = reactive({ count: 0 });

const increment = () => {
  state.count++;
};
</script>
<!--===== Script Zone =-->
<template>
  <button @click="increment">Click to increment</button>
  {{ state.count }}
</template>

<!--===== CSS Zone =-->
<style></style>
