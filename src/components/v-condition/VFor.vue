<script setup>
import { ref } from 'vue'

const items = ref(['Old Item 1', 'Old Item 2', 'Old Item 3', 'Old Item 4'])

const addNewItem = () =>{
    const itemLegth = items.value.length+1
    items.value.push('New Item' + itemLegth)
}

</script>

<template>
  <ul>
    <button @click="addNewItem()">Add New Item</button>
    <br>
    <br>
    <li v-for="item in items">
      {{ item }}
    </li>
  </ul>
</template>