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
      <div class="group"></div>
      <div class="about">
         <p class="logo"></p>
         <p class="aboutus">ABOUT US</p>
         <p class="heading">Great Digital Agency</p>
         <p class="description1">Our products are fully custom-made, built with the latest technologies and cloud-architectures.</p>
         <p class="description2">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam ex odio, turpis accumsan congue. Quisque blandit dui Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. In convallis porta mauris non aliquam.</p>
         <button class="get-started"> Get Started >></button>
      </div>
    </div>
    <div class="design"></div>
  </div>
</template>

<script setup>
// No script logic needed
</script>

<style scoped>
.page-wrapper {
  position: relative;
  width: 1920px;
  height: 1498px;
  background: #fff;
  overflow: hidden;
}

.left-svg-wrapper {
  position: absolute;
  left: -670.7px;
  top: 0;
  width: 1652px;
  height: 1316px;
  z-index: 1;
  overflow: visible;
}
.background-svg {
  width: 100%;
  height: 100%;
  object-fit: cover;
  pointer-events: none;
  user-select: none;
}

/* Right Side */
.login-form-wrapper {
  position: absolute;
  left: 981px;
  top: 0;
  width: 939px;
  height: 1080px;
  z-index: 2;
}

/* Group SVG background */
.group {
  position: absolute;
  left: 416.26px;
  top: 0;
  width: 718px;
  height: 720px;
  background: transparent url('@/assets/Group 35698.svg') no-repeat center center;
  background-size: contain;
  opacity: 1;
}

/* About Section */
.about {
  position: absolute;
  left: 97.99px;
  top: 480px;
  width: 700px;
}

.aboutus {
  position: absolute;
  left: 6px;
  height: 35px;
  text-align: left;
  font: normal normal 600 25px/50px Poppins;
  letter-spacing: 0px;
  color: #0E77FF;
  opacity: 1;
}
.heading {
  margin-top: 8px;
  text-align: left;
  width: 420px;
  height: 56px;
  margin-top: 48px;
  font: normal normal 600 40px/50px Poppins;
  letter-spacing: 0px;
  color: #000000;
  opacity: 1;
}
.description1 {
  margin-top: 42px;
  text-align: left;
  font: normal normal normal 22px/32px Poppins;
  letter-spacing: 0px;
  color: #000000;
  opacity: 1;
}
.description2 {
  margin-top: 10px;
  text-align: left;
  font: normal normal 300 18px/32px Poppins;
  letter-spacing: 0px;
  color: #000000;
  opacity: 1;
}
.get-started {
  margin-top: 32px;
  width: 239px;
  height: 72px;
  border: 2px solid #0E77FF;
  border-radius: 35px;
  opacity: 1;
  font: normal normal 600 18px/28px Poppins;
  border: none;
  cursor: pointer;
}

/* DESIGN SVG - Bottom Right */
.design {
  position: absolute;

  top: 760px;
  left: 1578px;
  width: 560px;
  height: 581px;

  background: transparent url('@/assets/Group 35650.svg') no-repeat center center;
  background-size: contain;
  opacity: 1;
  z-index: 3;
}
</style>