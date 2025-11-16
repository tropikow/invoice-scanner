<template>
  <div class="screen">
    <div class="public-container-login"></div>
    <div class="login-container">
      <span class="title-style">Welcome Back</span>
      <span class="span-style">Sign in to continue to your account</span>
      <span>Email Address</span>
      <InputRegular />
    </div>
  </div>
</template>
<style>
  .screen {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
  .public-container-login {
    background-color: #3b82f6;
    height: 100vh;
  }  
  .login-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;    
  }
  .title-style {
    font-weight: 700;
    font-size: xx-large;    
  }
  .span-style {
    color: #9ca3af;
  }
</style>