<template>
<div class="bground">
  <div v-for="j in 16" :key="j">
    <ul>
      <li  v-for="i in 18" :key="i" class="spot spot1" />
    </ul>
    <ul>
      <li  v-for="i in 16" :key="i" class="spot" />
    </ul>
  </div>
  <div class="namecard">
  <div class="circle circle2">平</div>
  <h2>陳子平<br><span>(Tzu-Ping Chen)</span></h2>
  <h5>前端工程師 / 量化交易者<br>andychentzupingwork@gmail.com</h5>
  <div class="square"></div>
  <div class="square"></div>
  <p>
    從事網頁前端工程師工作三年
    <br>
    <br>
    嘗試個人電子名片工作與網站架設服務
    <br>
    <br>
    <span class="red skill">擅長： Vue / Python</span>
    <br>
  </p>
  </div>
</div>
</template>

<script setup>
</script>

<style scoped>
*{
/*   border: solid 2px black; */
  font-family: 微軟正黑體;
  position: relative;
}

html,body{
  width: 100%; height: 100%;
  padding: 0px; margin: 0px;
}

body{
  background-color: #647f80;
  overflow: hidden;
  
}

ul {
    list-style: none;
    width: 100%;
    margin: 0;
    padding: 0;   
    overflow: hidden;
    white-space: nowrap;
}


.namecard{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);

  width: 250px; 
  height: 350px;
  margin-left: auto;
  margin-right: auto;
  border-radius: 7px;
  padding: 40px;
  padding-top: 100px;
  padding-bottom: 30px;
  
  letter-spacing: 1px;
  font-weight: 100;
  color: #4e6364;
  background-color: rgba(255,255,255,0.85);
  overflow: hidden;
  
  box-shadow: 10px 20px 15px -5px rgba(0,0,0,0.3);
  
}

.namecard h2{
  text-align: right;
  font-size: 25px;
  letter-spacing: 3px;
}

.namecard h2 span{
  font-size: 12px;
}

.namecard h5{
  height: 40px;
  text-align: right;
  line-height: 20px;
  color: #b34b4b;
  font-weight: 900;

}

.namecard p{
  font-size: 12px;
  font-weight: 500;
  color: #4e6364;
}

.red{
  color: #b34b4b;
  font-weight: 900;
}

.square{
  width: 100%; height: 10px;
  background-color: #647f80;
  
  font-size: 12px;
  color: white;
  text-align: center;
  padding-top: 2px;
}

.circle{

  border-radius: 100%;
  position: absolute;

  text-align: center;
  font-size: 40px;
  font-weight: 900;
  color: white;
  
}


.circle2{
  width: 50px; height: 50px;
  border: solid 0px #b34b4b;
  background-color: #e6b858;
  top: 40px;
  left: 40px;
}


.spot{
  display: inline-block;
  width: 50px; height: 50px;
 
  border-radius: 100%;
  background-color: #e6b858;
  margin: 30px;
  margin-top: 15px;
}

.spot1{
  left: -50px;
}

.bground{
  position: relative; /* ★ */
  width: 100%;
  height: 100vh;
  overflow: hidden;
}
</style>
