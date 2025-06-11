<script setup>
import SiteHeader from '~/components/Header.vue'
import TopBanner from '~/components/Banner.vue'
import InfoCard from '~/components/Card.vue'
import SiteFooter from '~/components/Footer.vue'
</script>

<template>
  <SiteHeader />
  <TopBanner />
  <main class="main-content">
    <h1>Привет, мир! 🌍</h1>
    <p>Давайте создадим что-то удивительное!</p>
    <section class="card-group">
      <InfoCard>Первая карта</InfoCard>
      <InfoCard>Вторая карта</InfoCard>
    </section>
  </main>
  <SiteFooter />
</template>

<style scoped>
.main-content {
  text-align: center; 
  padding: 3rem; 
}

.card-group {
  display: flex;
  justify-content: center;
  gap: 2rem; 
  margin-top: 2rem; 
  flex-wrap: wrap;
}
</style>
