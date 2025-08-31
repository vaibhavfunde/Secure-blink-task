

<template>
  <div class="home">
    <nav class="navbar">
      <div class="logo">Logo</div>
      <ul class="menu">
        <li>About</li>
        <li>Services</li>
        <li>Case Studies</li>
        <li>Testimonials</li>
        <li>Contact</li>
      </ul>
      <button class="login-btn" @click="goToLogin">
        <p>Login</p>
      </button>
    </nav>
    <div class="title"></div>
    <div class="herosectiondescription"></div>
    <button class="get-started" @click="goToLogin">
      <p>Get started &gt;&gt;</p>
    </button>
  </div>
  <HomeSecond/>
</template>

<script setup>
import { useRouter } from 'vue-router'
import HomeSecond from '../views/homesecond.vue'

const router = useRouter();
const goToLogin = () => {
  router.push('/login');
};
</script>

<style scoped>
.home {
  position: relative;
  width: 1920px;
  height: 1080px;
  background: url('@/assets/MaskGroup4.svg') no-repeat center center/cover;
  color: white;
  overflow: hidden;
}

/* Navbar */
.navbar {
  position: absolute;
  top: 67px;
  left: 281px;
  width: 1358px;
  height: 53px;
  display: flex;
  align-items: center;
  background: transparent;
  justify-content: flex-start;
  box-sizing: border-box;
}

/* Logo */
.logo {
  width: 60px;
  height: 35px;
  font: normal normal normal 25px/38px Poppins;
  color: #fff;
  text-align: left;
  margin-right: 50px;
}

/* Menu */
.menu {
  position: absolute;
  
  left: 574px;
 
  display: flex;
  gap: 41px;
  list-style: none;
  font: normal normal normal 18px/27px Poppins;
  color: #fff;
  padding: 0;
  margin: 0;
}
.menu li {
 
  color: #fff;
  opacity: 1;
}


.menu li:nth-child(1) {
width: 54px;
height: 25px;

}

.menu li:nth-child(2) {
width: 74px;
height: 25px;
}

.menu li:nth-child(3) {
width: 117px;
height: 25px;
}

.menu li:nth-child(4) {
  width: 113px;
height: 25px;
}

.menu li:nth-child(5) {
width: 73px;
height: 25px;
}




/* Login Button */
.login-btn {
  position: absolute;

  left: 1199px;
  width: 159px;
  height: 53px;
  background: #fff;
  border-radius: 5px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  border: none;
}
.login-btn p {
  width: 47px;
  height: 25px;
  font: normal normal normal 18px/27px Poppins;
  color: #000;
  margin: 0;
}

/* Title */
.title {
  position: absolute;
  top: 280px;
  left: 226px;
  width: 707px;
  height: 197px;
  background: transparent url('@/assets/title.svg') 0% 0% no-repeat padding-box;
  opacity: 1;
}

/* Hero Section Description */
.herosectiondescription {
  position: absolute;
  top: 526px;
  left: 225px;
  width: 735px;
  height: 75px;
  background: transparent url('@/assets/herosectiondescription.svg') 0% 0% no-repeat padding-box;
  opacity: 1;
}

/* Get Started Button */
.get-started {
  position: absolute;
  top: 641px;
  left: 225px;
  width: 239px;
  height: 72px;
  background: #fff;
  border-radius: 50px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  border: none;
}
.get-started p {
  font: normal normal normal 25px/31px Muli;
  color: #000;
  text-align: center;
  margin: 0;
}
</style>