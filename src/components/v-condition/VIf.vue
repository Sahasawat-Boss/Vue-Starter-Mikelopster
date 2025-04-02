<script setup>
import { ref } from 'vue'

const isChecked = ref(false)

</script>

<template>
    <div>
        <div>
            <input type="checkbox" v-model="isChecked">
            ติ๊กถูกเพื่อแสดงผล
        </div>
        <div v-if="isChecked">
            Checkbox is checked!
        </div>
    </div>
</template>