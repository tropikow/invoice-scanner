<script setup lang="ts">
  const options = [
    'dashboard',
    'invoices',
    'reports',
    'settings'
  ]
</script>
<template>
  <div class="header-container">
    <div class="header-container-content">
      <UtilsLogo />
      <span class="header-container-option" v-for="option in options">{{ option }}</span>      
      <ButtonRegular title="Help" />
    </div>
    <UtilsDivider />    
  </div>
</template>
<style scoped>
  .header-container {
    display: flex;    
    flex-direction: column;    
  }
  .header-container-content {
    display: flex;    
    justify-content: space-between;
    align-items: center;    
    padding: 20px;
  }
  .header-container-option {
    font-size: small;
    font-weight: 500;
    text-transform: capitalize;
    cursor: pointer;
  }
</style>