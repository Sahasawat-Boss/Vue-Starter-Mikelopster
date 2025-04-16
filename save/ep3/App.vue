<script setup>
import { ref, computed } from 'vue'
const firstName = ref('')
const lastName = ref('')
const fullName = computed(() => {
    return `${firstName.value} ${lastName.value}`
})
</script>

<template>
    <div>
        <div>Your fullname: {{ fullName }}</div>
        <div>
            Firstname <input type="text" v-model="firstName">
        </div>
        <div>
            Lastname <input type="text" v-model="lastName">
        </div>
    </div>
</template>