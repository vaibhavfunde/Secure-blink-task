<template>
  <div class="services-section">
    <div class="left-panel">
      <div class="title-box">
      <div class="arrow-icon"></div>
        <span class="services-label">
         
          OUR SERVICES
        </span>
        <h2>Transforming your ideas<br>into Reality</h2>
      </div>
      <div class="categories">
        <button>Web Development</button>
        <button>Mobile Development</button>
        <button class="active">UI/UX Designing</button>
        <button>Branding</button>
        <button>Cloud Technology</button>
      </div>
    </div>
    <div class="right-panel">
      <div class="card">
        <div class="icon-title">
          
          <h3>UI/UX Designing</h3>
        </div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
        <ul class="check-list">
          <li><span class="check">&#10003;</span> Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
          <li><span class="check">&#10003;</span> Lorem ipsum dolor sit amet, consectetur.</li>
          <li><span class="check">&#10003;</span> Lorem ipsum dolor sit amet, consectetur.</li>
          <li><span class="check">&#10003;</span> Lorem ipsum dolor sit amet, consectetur.</li>
        </ul>
      </div>
      <div class="blue-bg"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ServicesSection'
}
</script>

<style scoped>
.services-section {
  display: flex;

width: 1920px;
height: 889px;
}

.left-panel {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding-left: 60px;
  top: 242px;
  background: #fff;
}

.title-box {
  margin-bottom: 32px;
  
}

.services-label {
  position: absolute;
  left: 325px;

height: 35px;
/* UI Properties */
text-align: left;
font: normal normal 600 25px/50px Poppins;
letter-spacing: 0px;
color: #0E77FF;
opacity: 1;
}
.arrow-icon {
  position: absolute;
  left: 280px;
  width: 38px;
  height: 47px;
  background: transparent url('@/assets/Group 35624 (1).svg') 0% 0% no-repeat padding-box;
  opacity: 1;
}

h2 {
margin-top:50px;
position: absolute;
left: 280px;
width: 500px;
height: 156px;
/* UI Properties */
text-align: left;
font: normal normal 600 40px/50px Poppins;
letter-spacing: 0px;
color: #000000;
opacity: 1;
}

.categories {
position:relative;
  
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  max-width: 500px; /* increase width to fit two buttons per row */
  top: 211px;
}

.categories button {

left: 220px;
  position: relative;
  flex-basis: 48%; /* two buttons per row */
  width: 239px;
  height: 61px;
  background: #16B2FF17 0% 0% no-repeat padding-box;
  border-radius: 16px;
  border: none;
  opacity: 1;
  text-align: left;
  font-family: 'Poppins', sans-serif;
  font-weight: 600;
  font-size: 20px;
  line-height: 50px;
  letter-spacing: 0px;
  color: #0E77FF;
  margin-bottom: 12px;
  cursor: pointer;
  
}

.categories .active {
  background: #267DFF;
  color: #fff;
  box-shadow: 0 2px 12px rgba(38,125,255,0.15);
}

.right-panel {
  flex: 1;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  min-width: 350px;
}



.card {
    left: 124px;
    top: 26px;
  background: #fff;
  box-shadow: 0 6px 32px rgba(38,125,255,0.08);
  border-radius: 18px;
  padding: 36px 28px 36px 36px;
  width: auto;
  height: 450px;
  position: relative;
 
  margin-left: 48px;
 
}

.icon-title {
  display: flex;
  align-items: center;
width: 361px;
height: 61px;
z-index:6;
}

.icon-title h3 {


height: 61px;
/* UI Properties */
text-align: left;
font: normal normal 600 44px/110px Poppins;
letter-spacing: 0px;
color: #000000;
opacity: 1;
z-index:6;
}

.card p {
top:48px;
position:relative;
  width: 500px;

/* UI Properties */
text-align: left;
font: normal normal normal 16px/30px Poppins;
letter-spacing: 0px;
color: #000000;
opacity: 1;
z-index:6;
}

.check-list {
margin-top: 48px;

width: 454px;
height: 23px;
}

.check-list li {
position: relative;
  z-index: 6;
  color: #222;
  font-size: 0.98rem;
  margin-bottom: 10px;
  display: flex;
  align-items: center;
  left: -50px;
}

.check {
  display: inline-block;
  color: #28d97c;
  font-size: 1.2em;
  font-weight: bold;
  margin-right: 10px;
}

.blue-bg {
  position: absolute;
  right: 0;
  top: 0;
  bottom: 0;
width: 502px;
height: 889px;
transform: matrix(1, 0, 0, 1, 0, 0);
/* UI Properties */
background: #0E77FF 0% 0% no-repeat padding-box;
opacity: 1;
  z-index: 4 ;
  border-top-right-radius: 0;
  border-bottom-right-radius: 0;
}
</style>