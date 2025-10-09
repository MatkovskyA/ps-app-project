<script setup>
import { computed } from 'vue';
import Button from './components/button/Button.vue';
const ident = 'fla';

const colorClass = computed(() => {
  return ident === 'flag' ? 'red' : 'blue';
})

</script>

<template>
  <header>Logo</header>
  <main :id="ident" :class="colorClass">Content</main>
  <div>

  </div>
  <footer>
    <Button>
      <template #icon>+</template>
      Сохранить
      <template #minus>-</template>
      <template #[ident]>!!!</template>
    </Button>
  </footer>
</template>

<style scoped>
.red {
  color: red;
}

.blue {
  color: blue;
}
</style>
