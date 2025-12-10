<script setup lang="ts">
  const isSecurePassword = ref<boolean>(true);
  const changeSecurePassword = () => {
    isSecurePassword.value = !isSecurePassword.value;
  };
</script>
<template>
  <div class="container-grid-columns">
    <div class="container-grid-column-left">
      <div class="container-grid-column-left-header">
        <UtilsLogo spanColor='white' />
        <h1>Streamline your invoicing.</h1>
        <span>Scan, process, and manage all your invoices in one secure place</span>
      </div>
      <div class="container-grid-column-left-footer">
        <span>Scan, process, and manage all your invoices in one secure place</span>      
      </div>
    </div>    
    <div class="container-grid-column-right">
      <div class="container-grid-column-right_content">
        <h2>Welcome Back</h2>
        <span>Sign in to continue to your account.</span>
        <div class="container-grid-column-right_form">
          <span>Email Address</span>
          <InputRegular placeholder="Enter your email" type="mail" />          
          <span>Password</span>
          <InputRegular placeholder="Enter your password" type="password" :secureText="isSecurePassword" @click:secureText="changeSecurePassword" />
        </div>
        <div class="container-grid-column-right_second_actions">
          <div class="container-grid-column-right_second_actions_remember-me">
            <input type="checkbox"/>
            <span>Remember me</span>
          </div>
          <ButtonLink title='Forgot password?' />
        </div>
        <ButtonRegular title="Sign In" />
        <div>
          <span>Don't have an account?</span>
          <ButtonLink title="Sign Up" redirectTo="/auth/signup" />
        </div>
        <div class="container-grid-column-right_tyc">
          <ButtonTag>Terms of Service · Privacy Policy</ButtonTag>          
        </div>
      </div>
    </div>
  </div>
</template>
<style>
  h1 {
    color: white;
    font-size: 48px;
  }  
  h2 {
    font-size: 38px;
    font-weight: bold;
  }
  .container-grid-columns {
    display: grid;
    grid-template-columns: repeat(3, 1fr);    
  }
  .container-grid-column-left {        
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100vh;
    background-color: var(--colorBlue);
  }
  .container-grid-column-left span {
    color: white;
    font-size: 16px;
    opacity: 0.8;
  }
  .container-grid-column-left-header {
    display: flex;
    flex-direction: column;
    gap: 20px;
    padding: 20px;
  }
  .container-grid-column-left-footer {
    padding: 20px;
  }
  .container-grid-column-right {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;    
    height: 100vh;    
    grid-column: 2 / span 3;
  }
  .container-grid-column-right_content {
    display: flex;
    flex-direction: column;
    gap: 25px;
    width: 400px; 
  }  
  .container-grid-column-right_content > span{
    color: #94a3b8;
  }
  .container-grid-column-right_form {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .container-grid-column-right_second_actions {
    display: flex;
    justify-content: space-between;
  }
  .container-grid-column-right_second_actions_remember-me {
    display: flex;
    gap: 10px;
  }
  .container-grid-column-right_tyc {
    text-align: center;
  }
</style>