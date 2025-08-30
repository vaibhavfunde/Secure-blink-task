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
     <div class="title"> </div>

      <div class="herosectiondescription"> </div> 
      <button class="get-started" @click="goToLogin">
        <p>Get started >></p>
      </button>

  </div>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();
const goToLogin = () => {
  router.push('/login');
};
</script>

<style scoped>
:global(html, body) {
  margin: 0;
  padding: 0;
  height: 100%;
}

.home {
  background: #0d6efd;
  background: url('@/assets/MaskGroup4.svg') no-repeat center center/cover;
  color: white;
  height: 100vh;
}

.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  position:relative;
 
  background-color: transparent;

  box-sizing: border-box;
  top: 67px;
  left: 281px;
  right:281px;
width: 1008px;
height: 53px;
}

.logo {
  
  
  
  width: 60px;
  height: 35px;
  /* UI Properties */
  text-align: left;
  font: normal normal normal 25px/38px Poppins;
letter-spacing: 0px;
color: #FFFFFF;
opacity: 1;
}

.menu {

  display: flex;
  gap: 41px;
  list-style: none;
 top: 80px;


height: 25px;
text-align: left;
font: normal normal normal 18px/27px Poppins;
letter-spacing: 0px;
color: #FFFFFF;
opacity: 1;
  right:281px;


}
.menu li:first-child {
  margin-left: 57px;
}

.menu li {
 text-align: left;
font: normal normal normal 18px/27px Poppins;
letter-spacing: 0px;
color: #FFFFFF;
opacity: 1;

}

.login-btn {
 
 top: 67px;

width: 159px;
height: 53px;
 cursor: pointer; 
  border-radius: 50px;
   align-items: center;
/* UI Properties */
background: #FFFFFF 0% 0% no-repeat padding-box;
border-radius: 5px;
opacity: 1;
 border-radius: 5px; 

display: flex;       /* For centering text */
  justify-content: center;
  align-items: center;
}

.login-btn p {
 top: 80px;

width: 47px;
height: 25px;
/* UI Properties */


font: normal normal normal 18px/27px Poppins;
letter-spacing: 0px;
color: #000000;
opacity: 1;
}

.hero {

  margin-top: 80px;
  text-align: center;

}
.title{
  position: absolute;
  top: 205px;
  left: 226px;
width: 707px;
height: 197px;
/* UI Properties */
background: transparent url('@/assets/title.svg') 0% 0% no-repeat padding-box;
opacity: 1;
}

.herosectiondescription{
  position: absolute;
  top: 426px;
  left: 225px;
  width: 735px;
  height: 75px;
  /* UI Properties */
background: transparent url('@/assets/herosectiondescription.svg') 0% 0% no-repeat padding-box;
opacity: 1;
}

.get-started {
position : absolute;
 top: 520px;
left: 225px;
width: 239px;
height: 72px;
 border-radius: 50px;
/* UI Properties */
background: #FFFFFF 0% 0% no-repeat padding-box;
opacity: 1;
cursor: pointer;
}
.get-started p{
text-align: center;
font: normal normal normal 25px/31px Muli;
letter-spacing: 0px;
color: #000000;
opacity: 1;

}
</style>