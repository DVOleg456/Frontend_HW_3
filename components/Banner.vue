<template>
    <div class="banner" :style="{ backgroundColor: color }">
      <div class="container">
        <h2>{{ title }}</h2>
        <p>{{ description }}</p>
      </div>
    </div>
  </template>

<style scoped>
.banner {
    font-family: $secondary-font;
    font-weight: 600;
}
</style>

<script setup>
defineProps({
    title: String,
    description: String,
    color: {
      type: String,
      default: '#4CAF50'
    }
})
</script>