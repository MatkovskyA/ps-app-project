<script setup>
  const props = defineProps({
      label: {
        type: String,
        default: 'No written',
      },
      stat: {
        type: String,
        default: undefined,
      }
    })
</script>

<template>
  <div class="stat">
    <div class="stat-name font-bold">{{ props.label }}</div>
    <div class="stat-value font-medium">{{ props.stat }}</div>
  </div>
</template>

<style scoped>
  .stat {
    font-size: 28px;
    display: flex;
    justify-content: space-between;
  }

  .stat-name {
    font-weight: 700px;
    text-transform: uppercase;
  }

  .stat-value {
    font-weight: 500px;
  }
</style>
