<template>
    <div class="container">
      <h1>Iniciar sesión</h1>
      <form>
        <div class="input-container">
          <label for="username">Nombre de usuario:</label>
          <input type="text" id="username" name="username" v-model="username" required />
          <div class="input-background"></div>
        </div>
        <div class="input-container">
          <label for="password">Contraseña:</label>
          <input type="password" id="password" name="password" v-model="password" required />
          <div class="input-background"></div>
        </div>
        <div class="button-container">
          <button type="submit" class="primary">Iniciar sesión</button>
        </div>
      </form>
      <div class="links">
        <a href="#">¿Olvidaste tu contraseña?</a>
      </div>
    </div>
  </template>
  
  <style>
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  
  form {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2rem;
    border-radius: 30px;
    background-color: #f0f3f5;
    box-shadow: 20px 20px 60px #c9d1d9, -20px -20px 60px #ffffff;
  }
  
  .input-container {
    position: relative;
    margin: 1rem 0;
  }
  
  label {
    position: absolute;
    top: -1.2rem;
    left: 0.8rem;
    font-size: 1rem;
    color: #808080;
  }
  
  input {
    width: 100%;
    height: 3rem;
    padding: 0.5rem 0.8rem;
    border: none;
    outline: none;
    border-radius: 15px;
    background-color: #f0f3f5;
  }
  
  .input-background {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
    height: 3rem;
    background-color: #c9d1d9;
    border-radius: 15px;
    z-index: -1;
  }
  
  .button-container {
    margin-top: 2rem;
  }
  
  button {
    width: 100%;
    height: 3rem;
    border: none;
    border-radius: 15px;
    background-color: #5d5fe5;
    color: #fff;
    font-size: 1.2rem;
    cursor: pointer;
  }
  
  .primary {
    background-color: #5d5fe5;
  }
  
  .links {
    margin-top: 1rem;
  }
  
  a {
    color: #808080;
    font-size: 0.8rem;
    text-decoration: none;
  }
  
  a:hover {
    text-decoration: underline;
  }
  </style>
  
  <script>
  export default {
    data() {
      return {
        username: "",
        password: "",
      };
    },
  };
  </script>
  