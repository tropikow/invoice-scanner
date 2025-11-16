<script setup lang="ts">
  const props = withDefaults(defineProps<{
    size?: string;
    color?: string;    
  }>(),{ size: '20px', color: 'currentColor' })
</script>
<template>
  <svg :width="size" :height="size" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path 
      d="M4 4H17.3334V17.3334H30.6666V30.6666H44V44H4V4Z" 
      :fill="color"
    />
  </svg>
</template>