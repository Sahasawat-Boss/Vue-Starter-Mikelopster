<script setup>//<<-- This show that what will it show first
import { ref } from 'vue'//<<-- Only function ref from vie
import Card from './components/Card.vue'

const counter = ref(0) //<<-- counter contain variable of 0

const message = "Boss"

const cards = [
  {
    title: "Welcome to Vue",
    description: "Vue.js is a progressive framework for building user interfaces.",
    imageUrl: "https://picsum.photos/id/1/300/200"
  },
  {
    title: "Learn Components and Basic",
    description: "Components are reusable Vue instances with a name.",
    imageUrl: "https://picsum.photos/id/2/300/200"
  }
]
</script>
<!--===== Script Zone =-->

<template>
  <div class="app-container">
    <header class="app-header">
      <h1>Vue Card Demo</h1>
      <div class="counter-display">Counter: {{ counter }}</div>
    </header>

    <div class="hello">Test</div>
    
    <div class="cards-container">
      <Card 
        v-for="(card, index) in cards" 
        :key="index"
        :title="card.title"
        :description="card.description"
        :imageUrl="card.imageUrl"
      />
    </div>

    <footer class="app-footer hello">
      Hello {{ message }}
    </footer>
  </div>
</template>


<!--===== CSS Zone =-->
<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
}

.app-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 2rem;
}

.app-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 2rem;
  padding-bottom: 1rem;
  border-bottom: 1px solid #eee;
  color: #000;
}

.counter-display {
  background-color: #333;
  color: white;
  padding: 0.5rem 1rem;
  border-radius: 4px;
}

.cards-container {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: center;
}

.app-footer {
  margin-top: 2rem;
  padding-top: 1rem;
  border-top: 1px solid #eee;
  text-align: center;
  color: #666;
}

.hello {
  background-color: blue;
  color: aqua;
}
</style>