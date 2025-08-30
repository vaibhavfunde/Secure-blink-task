<template>
  <div class="login-container">
    <div class="login-box">
      <h2>Login</h2>
      <form>
        <input type="email" placeholder="Email" required />
        <input type="password" placeholder="Password" required />
        <button type="submit">Login</button>
      </form>
    </div>
  </div>
</template>

<style scoped>
.login-container {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;

  /* Background image */
  background: url('@/assets/MaskGroup4.svg') no-repeat center center/cover;
}

.login-box {
  background: rgba(255, 255, 255, 0.9);
  padding: 30px;
  border-radius: 12px;
  text-align: center;
}
.login-box input {
  display: block;
  margin: 10px auto;
  padding: 10px;
  width: 200px;
}
.login-box button {
  margin-top: 10px;
  padding: 10px 20px;
  cursor: pointer;
}
</style>
