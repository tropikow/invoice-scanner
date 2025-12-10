<script setup lang="ts">
  const props = withDefaults(defineProps<{
    title: string
  }>(), {})
</script>
<template>
  <button>
    <span>{{ title }}</span>    
  </button>
</template>
<style scoped>
  button {
    background-color: transparent;
    color:#607AFB;
    border: none;
    outline: none;
    font-weight: 700;
    cursor: pointer;
  }
  button:hover {
    text-decoration: underline;
    text-decoration-color: inherit;
    text-decoration-thickness: 1px;
  }
</style>