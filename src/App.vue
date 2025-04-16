<script setup>
import { ref, watch } from 'vue'
const message = ref('')
const uppercaseMessage = ref('')

watch(message, (newMessage) => {
    uppercaseMessage.value = newMessage.toUpperCase()
})
</script>

<template>
    <div>
        <input type="text" v-model="message">
        <p>Uppercase Message: {{ uppercaseMessage }}</p>
    </div>
</template>