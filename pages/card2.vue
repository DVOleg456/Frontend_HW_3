<template>
    <div>
      <Header />
      <Banner 
        title="Фреймворк Nuxt.js" 
        description="Разработка современных приложений на Vue.js с SSR и удобной маршрутизацией." 
        color="#2196F3"
      />
      <div class="card2-content">
        <h2>Описание темы</h2>
        <p>
        Nuxt.js — фреймворк для Vue.js, который позволяет:<br>
        - Создавать SEO-оптимизированные приложения благодаря SSR (Server-Side Rendering).<br>
        - Использовать автоматическую маршрутизацию через папку `pages/`.<br>
        - Интегрировать TypeScript и другие инструменты из коробки.
      </p>
      </div>
    </div>
  </template>
  
  <style>
  .card2-content {
    padding: 2rem;
    max-width: 800px;
    margin: 0 auto;
  }
  </style>