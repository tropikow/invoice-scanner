<script setup lang="ts">
  const props = withDefaults(defineProps<{
    spanColor?: string;
  }>(), { spanColor: 'black' })
</script>
<template>
  <div class="logo-container">
    <IconsRegularLogo color="#607AFB" />
    <spa class="logo-container-title" :style="{color: spanColor}" >InvoiceScanner</spa>
  </div>
</template>
<style scoped>
  .logo-container {
    display: flex;    
    align-items: center;
    gap: 10px;    
  }
  .logo-container-title {
    font-weight: 700;
  }
</style>