<template>
    <div class="card" :style="{ backgroundColor: color }">
      <h3>{{ title }}</h3>
      <p>{{ description }}</p>
      <NuxtLink :to="to" class="card-button">Узнать больше</NuxtLink>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    description: String,
    color: {
      type: String,
      default: '#FF9800'
    },
    to: { 
      type: String,
      required: true
    }
  })
  </script>
  
  <style scoped>
  @import '~/assets/styles/variables.scss';
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
  
  .card-button {
    color: $primary-color;
    padding: 0.5rem 1rem;
    border-radius: 4px;
    transition: all 0.3s ease;
  }
  
  .card-button:hover {
    background-color: $primary-color;
    color: white;
  }
  </style>