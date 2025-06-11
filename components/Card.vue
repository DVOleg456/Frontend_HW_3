<template>
  <div class="custom-card">
    <slot>Card Content</slot>
  </div>
</template>

<style lang="scss" scoped>
@use '@/assets/styles/mixins.scss' as mixin;

.custom-card {
  @include mixin.card-style(blue);
  font-family: 'Times New Roman', sans-serif;
  border-radius: 15px;
  padding: 1.5rem;
}
</style>
