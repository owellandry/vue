<template>
  <div class="login-container">
    <form class="login-form">
      <h1 class="login-title">Iniciar sesión</h1>
      <div class="login-inputs">
        <input type="text" class="input" placeholder="Usuario" />
        <input type="password" class="input" placeholder="Contraseña" />
        <a href="#" class="forgot-password">Recuperar contraseña</a>
        <button class="btn">Ingresar</button>
      </div>
    </form>
  </div>
</template>


<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
.login-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #252934;
}

.login-form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 400px;
  padding: 40px;
  border-radius: 20px;
  background-color: rgba(255, 255, 255, 0.15);
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
}

.login-title {
  font-family: "Helvetica Neue", sans-serif;
  margin-bottom: 30px;
  color: #fff;
  text-align: center;
  font-size: 28px;
  font-weight: bold;
  text-shadow: 0px 2px 3px rgba(0, 0, 0, 0.3);
}

.login-inputs {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.input {
  width: 100%;
  padding: 10px;
  margin-bottom: 20px;
  border: none;
  border-radius: 5px;
  background-color: rgba(255, 255, 255, 0.1);
  color: #fff;
  font-size: 16px;
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
}

.forgot-password {
  align-self: center;
  cursor: pointer;
  margin-bottom: 20px;
  color: #fff;
  text-shadow: 0px 2px 3px rgba(0, 0, 0, 0.3);
  font-size: 20px;
  text-decoration: none;
}

.btn {
  width: 100%;
  padding: 10px;
  margin-top: 10px;
  border: none;
  border-radius: 5px;
  background-color: #fff;
  color: #252934;
  font-size: 16px;
  font-weight: bold;
  text-transform: uppercase;
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
  transition: all 0.3s ease-in-out;
}

.btn:hover {
  background-color: #252934;
  color: #fff;
  box-shadow: 0 8px 45px 0 rgba(31, 38, 135, 0.57);
  cursor: pointer;
}

</style>