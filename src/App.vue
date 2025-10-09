<script setup>
import Button2 from './components/button-2/Button2.vue';
</script>

<template>
  <main class="main">
    <Button2>
      <slot>
        Начать игру
      </slot>
    </Button2>
  </main>
</template>

<style scoped>
  .main {
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
  }
</style>
