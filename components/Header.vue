<template>
    <header class="header">
      <div class="container">
        <h1>Мой Nuxt-проект</h1>
        <nav>
          <NuxtLink to="/" class="nav-link">Главная</NuxtLink>
          <NuxtLink to="/card1" class="nav-link">Основы веб-разработки</NuxtLink>
          <NuxtLink to="/card2" class="nav-link">Фреймворк Nuxt.js</NuxtLink>
        </nav>
      </div>
    </header>
  </template>
  
  <script setup>

  </script>
  
  <style scoped>
  .header {
    background-color: #4CAF50;
    padding: 1rem 0;
    color: white;
  }
  
  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 15px;
  }
  
  .nav-link {
    margin-left: 20px;
    color: white;
    text-decoration: none;
    font-weight: bold;
  }
  
  .nav-link:hover {
    text-decoration: underline;
  }
  </style>