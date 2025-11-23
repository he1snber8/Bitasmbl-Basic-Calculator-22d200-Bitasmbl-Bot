<template>
  <div class="display">
    <div class="prev">{{ previous }}</div>
    <div class="current">{{ current }}</div>
  </div>
</template>

<script setup lang="ts">
defineProps<{ previous: string; current: string }>()
</script>

<style scoped>
.display { padding:1rem; background:#222; color:#fff; text-align:right; }
.prev { font-size:.8rem; opacity:.7; }
.current { font-size:1.6rem; }
</style>