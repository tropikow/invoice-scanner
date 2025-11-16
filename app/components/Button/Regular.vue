<script setup lang="ts">
  type VariantButton = 'primary' | 'secondary' | 'option';
  const props = withDefaults(defineProps<{
    title: string;
    variant?: VariantButton;
  }>(), { variant: 'primary' })
</script>
<template>
  <button :class="[
    variant === 'primary' ? 'primary-style' : 'secondary-style'
  ]">
    {{ title }}
  </button>
</template>
<style scoped>
  button {
    background-color: #607AFB;
    color: white;
    border: none;
    outline: none;
    padding: 5px 15px;
    border-radius: 5px;
    cursor: pointer;
    height: 30px;    
    font-weight: 700;
  }
  .primary-style {
    background-color: #607AFB;
  }
  .primary-style:hover {
    background-color: #5c75f2;
  }
  .secondary-style {
    background-color: white;
    border: 1px solid #d1d5db;
    color: black;
    font-weight: 700;
  }
</style>