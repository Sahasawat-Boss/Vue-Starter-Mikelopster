<script setup>
import { reactive } from 'vue' //Concept reactive

defineProps({
    msg: String,
})

const counter = reactive({ count: 0}) //store reactive 0 >> when Update >> change html 

const increase = () => {
    counter.count = counter.count + 1
}
</script>

<template>
    <div>
        <div>Hello Comps</div>
        <div>Couter {{ counter.count }}</div>
        <button @click="increase">Add Couter</button>
    </div>

</template>

<style scoped>
.read-the-docs {
    color: #888;
}
</style>
