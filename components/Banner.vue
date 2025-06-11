<template>
  <section class="custom-banner">
    <p>Введение в Nuxt</p>
  </section>
</template>

<style lang="scss" scoped>
@use '@/assets/styles/mixins.scss' as mixin;

.custom-banner {
  @include mixin.card-style(purple);
  font-family: 'Times New Roman', sans-serif;
  padding: 2rem;
  text-align: center;
}
</style>
