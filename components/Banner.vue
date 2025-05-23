<template>
  <div class="banner" :class="{ 'gradient': true }" :style="{ backgroundColor: color }">
    <div class="container">
      <h2>{{ title }}</h2>
      <p>{{ description }}</p>
    </div>
  </div>
</template>

<style scoped>
@import '@/assets/styles/variables.scss';

.banner {
  padding: 4rem 0;
  text-align: center;
  color: white;
  font-family: $secondary-font;
}

.gradient {
  @include gradient(v-bind(color));
}
</style>