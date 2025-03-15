<script setup>//<<-- This show that what will it show first
import { ref } from 'vue'//<<-- Only function ref from vie

const counter = ref(0) //<<-- counter contain variable of 0

const message = "Boss"
</script>
<!--===== Script Zone =-->

<template>
  <div>
    Counter {{ counter }}
  </div>

  <div class="hello">
    Hello {{ message }}
    Hello {{ message }}
  </div>
</template>


<!--===== CSS Zone =-->
<style>
.hello {
  background-color: blue;
  color: aqua;
}
</style>