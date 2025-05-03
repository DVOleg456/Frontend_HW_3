<template>
    <div>
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
          :card-color="card.color"
          :to="card.to"
        />
      </div>
    </div>
  </template>
  
  <script setup>
  const cards = [
    {
      id: 1,
      title: "Основы веб-разработки",
      description: "HTML для структуры, CSS для дизайна, JavaScript для интерактивности.",
      color: "#FFA500",
      to: "/card1"
    },
    {
      id: 2,
      title: "Фреймворк Nuxt.js",
      description: "Разработка современных приложений на Vue.js с SSR и удобной маршрутизацией.",
      color: "#2196F3",
      to: "/card2"
    }
  ]
  </script>
  
  <style>
  .card-container {
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    justify-content: center;
    padding: 2rem;
  }
  
  .card {
    flex: 1 1 300px;
  }
  </style>