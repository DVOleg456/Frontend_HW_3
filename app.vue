<template>
  <Header />
  <Banner 
    title="Добро пожаловать!" 
    description="Это мой первый Nuxt-проект." 
    color="#4CAF50"
  />
  <div class="card-container">
    <Card 
      v-for="card in cards" 
      :key="card.id" 
      :title="card.title" 
      :description="card.description" 
      :color="card.color"
    />
  </div>
  <Footer />
</template>

<script setup>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import Card from '@/components/Card.vue'
import Banner from '@/components/Banner.vue'

const cards = [
  {
    id: 1,
    title: "Основы веб-разработки",
    description: "HTML для структуры, CSS для дизайна, JavaScript для интерактивности.",
    color: "#FFA500"
  },
  {
    id: 2,
    title: "Фреймворк Nuxt.js",
    description: "Разработка современных приложений на Vue.js с SSR и удобной маршрутизацией.",
    color: "#2196F3"
  }
]
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat :wght@400;700&family=Open+Sans:wght@400;600&display=swap');

body {
  font-family: 'Open Sans', sans-serif;
}
</style>