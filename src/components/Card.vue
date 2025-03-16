<script setup>
import { ref } from 'vue';

const props = defineProps({
  title: {
    type: String,
    default: 'Card Title'
  },
  description: {
    type: String,
    default: 'This is a description of the card content. You can customize this text.'
  },
  imageUrl: {
    type: String,
    default: 'https://picsum.photos/300/200'
  }
});

const likes = ref(0);

const incrementLikes = () => {
  likes.value++;
};
</script>

<template>
  <div class="card">
    <img :src="imageUrl" alt="Card image" class="card-image">
    <div class="card-content">
      <h2 class="card-title">{{ title }}</h2>
      <p class="card-description">{{ description }}</p>
      <div class="card-actions">
        <button @click="incrementLikes" class="like-button">
          ❤️ {{ likes }}
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  transition: transform 0.3s ease;
  max-width: 350px;
  margin: 1rem;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
}

.card-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.card-content {
  padding: 1.5rem;
}

.card-title {
  margin: 0 0 0.5rem 0;
  color: #333;
  font-size: 1.5rem;
}

.card-description {
  color: #666;
  margin-bottom: 1.5rem;
  line-height: 1.5;
}

.card-actions {
  display: flex;
  justify-content: flex-end;
}

.like-button {
  background-color: #f8f9fa;
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 0.5rem 1rem;
  cursor: pointer;
  display: flex;
  align-items: center;
  gap: 0.5rem;
  transition: all 0.2s ease;
}

.like-button:hover {
  background-color: #f1f3f5;
  border-color: #c8c9ca;
}
</style> 