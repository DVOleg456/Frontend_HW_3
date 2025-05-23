<template>
  <div class="card" :style="{ backgroundColor: color }">
    <h3>{{ title }}</h3>
    <p>{{ description }}</p>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  description: String,
  color: {
    type: String,
    default: '#FF9800'
  }
})
</script>

<style scoped>
@import '@/assets/styles/variables.scss';

.card {
  border-radius: 8px;
  padding: 2rem;
  margin: $card-gap 0;
  text-align: center;
  font-family: $primary-font;
  color: white;
  transition: transform 0.3s ease;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}
</style>