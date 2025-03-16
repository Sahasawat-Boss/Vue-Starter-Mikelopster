<script setup>
import { ref } from 'vue'

const answer = ref('')

</script>

<template>
  <div>
    <input type="radio" value="yes" v-model="answer"> Yes
    <input type="radio" value="no" v-model="answer"> No
    <div v-if="answer === 'yes'">
      You answered Yes!
    </div>
    <div v-else-if="answer === 'no'">
      You answered No!
    </div>
    <div v-else>
      Please select an answer.
    </div>
  </div>
</template>