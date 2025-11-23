<template>
  <button class="btn" @click="$emit('press')">
    <slot />
  </button>
</template>

<script setup lang="ts">
defineEmits<{ (e:'press'): void }>()
</script>

<style scoped>
.btn { padding:1rem; font-size:1.2rem; border:1px solid #ccc; background:#f3f3f3; cursor:pointer; }
.btn:active { background:#e0e0e0; }
</style>