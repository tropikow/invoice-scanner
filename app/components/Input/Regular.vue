<script setup lang="ts">
  type EmittedDefine = 'secureText';
  const props = withDefaults(defineProps<{
    placeholder?: string;
    type?: string;
    secureText?: boolean;
  }>(), { type:'text', secureText: true });
  const emits = defineEmits([
    'click:secureText'
  ]);
  const handleEmit = (click: EmittedDefine) => {
    emits(`click:${click}`)
  };
</script>
<template>
  <div class="input-container">
    <input :placeholder="placeholder" :type="type" v-if="type !== 'password'" />  
    <input :placeholder="placeholder" :type="secureText === true ? 'password' : 'text'" v-else />  
    <div class="icon-container" v-if="type === 'password'" @click="handleEmit('secureText')">
      <IconsEye color="#64748b" v-if="secureText"/>
      <IconsEyeOff color="#64748b" v-else />
    </div>
  </div>
</template>
<style scoped>
  .input-container {        
    display: flex;
    justify-content: center;
    align-items: center;
    border: 1px solid #d1d5db;
    border-radius: 5px;
    overflow: hidden;
    padding: 5px;
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
  .icon-container {
    cursor: pointer;
  }
</style>