<script setup>
import Stat from './components/stat/Stat.vue';
import CitySelect from './components/citySelect/CitySelect.vue';

const data = {
  label: "Осадки",
  stat: "0%",
}

function getCity(city){
  console.log(city);
}
</script>

<template>
  <main class="main" :style="{ backgroundColor: currentColor}">
    <Stat label="Влажность" stat="90%" />
    <Stat v-bind="data" />
    <CitySelect @select-city="getCity"/>
  </main>
</template>

<style scoped>
  .main {
    padding: 60px 50px;
    border-radius: 25px;
    background: var(--color-bg-card);
  }

  .dog-generator {
    text-align: center;
    padding: 20px;
    max-width: 600px;
    margin: 0 auto;
  }
</style>
