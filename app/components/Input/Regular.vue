<template>
  <div class="input-container">
    <input placeholder="placeholder" />
  </div>
</template>
<style scoped>
  .input-container {
    width: 100%;
    height: 30px;
    padding: 10px;
    border: 1px solid #d1d5db;
    border-radius: 5px;
    overflow: hidden;
  }
  .input-container > input {
    width: 100%;
    height: 100%;
    border: none;
    outline: none;
  }
  .input-container > input::placeholder,
  textarea::placeholder {
    color: #6b7280;
    font-weight: 400;    
    font-size: 12px;
  }
</style>