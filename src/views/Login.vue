<template>
  <div class="page-wrapper">
    <!-- Left Side SVG Background -->
    <div class="left-svg-wrapper">
      <img
        src="@/assets/loginimage.svg"
        alt="Background SVG"
        class="background-svg"
      />
    </div>

    <!-- Right Side Login Form -->
    <div class="login-form-wrapper">
      <div class="login-form">
        <h2>Login to Access Dashboard</h2>
        <form @submit.prevent="handleLogin">
          <div>
            <label>Email*</label>
            <input v-model="email" type="email" required placeholder="Enter your email" />
          </div>
          <div>
            <div class="flex-between">
              <label>Password*</label>
              <a href="#" class="forgot-password">Forget Password?</a>
            </div>
            <input v-model="password" type="password" required placeholder="Enter your password" />
          </div>
          <button type="submit">Login <span>→</span></button>
        </form>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue"
import { useRouter } from "vue-router"

const email = ref("")
const password = ref("")
const router = useRouter()

const handleLogin = () => {
  if (email.value && password.value) {
    router.push("/dashboard")
  } else {
    alert("Please enter Email and Password")
  }
}
</script>

<style scoped>
.page-wrapper {
  position: relative;
  width: 1920px;
  height: 1080px;
  background: #fff;
  overflow: hidden;
}

/* Left SVG */
.left-svg-wrapper {
  position: absolute;
  top: -177.154296875px;
  left: -547.7056884765625px;
  width: 1652px;
  height: 1316px;
  z-index: 1;
  overflow: visible;
}

.background-svg {
  width: 100%;
  height: 100%;
  object-fit: cover;
  /* Prevent pointer interaction and selection */
  pointer-events: none;
  user-select: none;
}

/* Right login form */
.login-form-wrapper {
  position: absolute;
  top: 304px;
  left: 1319px;
  transform: translateY(-50%);
  width: 440px;
  z-index: 2;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  background: transparent;
}

.login-form {
  width: 100%;
  max-width: 400px;
  background: transparent;
  padding: 32px;
}

.login-form h2 {
width: 453px;  
text-align: left;
font: normal normal 600 32px/50px Poppins;
letter-spacing: 0px;
color: #000000;
opacity: 1;
}

.login-form label {

  left: 1312px;
  width: 92px;
  height: 26px;
  /* UI Properties */
  text-align: left;
  font: normal normal 600 18px/32px Poppins;
letter-spacing: 0px;
opacity: 1;
}

.login-form input {
  
  width: 353px;
  border: 1px solid #ccc;
  border-radius: 4px;
  padding: 0.75rem;
  margin-bottom: 1rem;
  font-size: 1rem;
  outline: none;
}

.flex-between {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.forgot-password {
  left: 1605px;
  color: #e53e3e;
  font-size: 0.9rem;
  text-decoration: underline;
  cursor: pointer;
}

.login-form button {
  width: 100%;
  background: #2563eb;
  color: #fff;
  padding: 0.75rem;
  border-radius: 999px;
  border: none;
  font-size: 1.1rem;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.2s;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 8px;
}

.login-form button:hover {
  background: #1e40af;
}
</style>