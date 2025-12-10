<script setup lang="ts">
  interface Props {
    to: string;
  }
  const props = defineProps([
    'redirectTo'
  ])  
</script>
<template>
  <div>
    <span>
      <NuxtLink :to="redirectTo">
        <slot />
      </NuxtLink>
    </span>
  </div>
</template>
<style scoped>
  span {
    font-size: 0.8rem;
    color: #64748b;
    cursor: pointer;    
  }
  span:hover {
    text-decoration: underline;
    text-decoration-color: inherit;
    text-decoration-thickness: 1px;
  }
</style>