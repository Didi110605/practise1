<script>
import image from "./assets/girl.png"
import imgGoogle from "./assets/logogoogle.png"
import imgNike from "./assets/logonike.png"
import imgSamsung from "./assets/logosamsung.png"
import imgApple from "./assets/logoApple.png"
import imgAdidas from "./assets/logoadidas.png"

export default{
  data: function(){
    return{
      image:image,
      imgGoogle: imgGoogle,
      imgNike: imgNike,
      imgSamsung: imgSamsung,
      imgApple: imgApple,
      imgAdidas: imgAdidas,

    }
  }
}
</script>

<template>
  <header>
   <h1 class="logo">Logo</h1>
   <div class="menu-container">
     <h2 class="menu">About</h2>
     <h2 class="menu">Work</h2>
     <h2 class="menu">Contact</h2>
   </div>
 </header>


   <div class="content-container">
     <div class="text-container">
       <p class="text1">Branding | Image making</p>
       <p class="text2">Visual Designer</p>
       <p class="text3">This is a template Figma file, turned into code using Anima. 
         <br/>
         Learn more at AnimaApp.com
       </p>
       <button class="button">Contact</button>
     </div>
     <img :src="image" class="image"> 
   </div>
   <div class="logosWraper">
      <img :src="imgGoogle"/>
      <img :src="imgNike"/>
      <img :src="imgSamsung"/>
      <img :src="imgApple"/>
      <img :src="imgAdidas"/>

    </div>



<footer>
    <div class="footerContent">
      <div class="footerText">
      <h3> Lets work together</h3>
      <p> This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com</p>

    </div>

    <form id="inputform" class="inputform">
      <input type="text" value="Name">
      <input type="email" value="Email">
      <input type="submit" class="inputSubmit" value="Submit">
    </form>
    </div>

  </footer>

</template>

<style scoped>
  header {
  display: flex;
  justify-content: space-between; 
  align-items: center; 
  padding: 20px 30px;
}

.logo {
  margin: 0; 
  text-align: left; 
  font-family: 'Arial', sans-serif;
  font-size: 20px;
}

.menu-container {
  display: flex;
  align-items: center; 
  text-align: right;
}

.menu {
  margin: 0 10px; 
  font-family: 'Arial', sans-serif;
  font-size: 17px;
  font-weight: 300;
}
.content-container {
  display: flex; 
  align-items: flex-start; 
  margin: 0 45px;
}

.text-container {
  margin-right: 20px; 
  flex: 1;
  margin-top: 30px;
}

.image {
  width: 100%; 
  max-width: 320px; 
  height: auto; 
  object-fit: cover; 
  margin-top: 40px;
  margin-right: 80px;
}



.text1 {
    margin: 0; 
    text-align: left; 
    font-family: 'Arial', sans-serif;
    font-size: 20px;
    font-weight: 600; 
    margin-left: 45px; 
    margin-top: 40px;
  }
.text2{
  margin: 0; 
    text-align: left;
    font-family: 'Arial', sans-serif;
    font-size: 68px;
    font-weight: 600; 
    margin-left: 45px; 
    margin-top: 20px;
}
.text3{
  text-align: left;
    font-family: 'Arial', sans-serif;
    margin: 0;
    font-size: 17px;
    margin-left: 45px; 
    margin-top: 20px;
}
.button {
    background-color:#2D2D2D; 
    color: white; 
    font-family: 'Arial', sans-serif; 
    font-size: 20px; 
    padding: 10px 20px; 
    border: none; 
    margin-left: 45px; 
    margin-top: 60px; 
    width: 211px;
    height: 78px;
}
  .logosWraper{
    margin-top: 20px; 
  margin-bottom: 20px; 
    height: auto;
    display: flex;
    justify-content: space-between;
    padding: 10px;
    img{
      height: 100%;
    }

  }
.footerContent {
  display: flex;
  justify-content: space-between;
  position: relative;
  bottom: 0;
  left: 0;
  width: 100%;
  padding: 20px; 
  background-color: white; 
}

.footerText {
  width: 500px; 
  margin-right: 5%; 
  padding: 10px; 
  line-height: 1.5; 
  font-size: 16px; 
  font-family: 'Arial', sans-serif;
}

.inputform {
  display: flex;
  flex-direction: column;
  gap: 15px; 
  width: 400px; 
  margin: 20px auto; 
  padding: 15px; 
  margin-right: 20px;
}

.inputform input {
  font-size: 16px; 
  background-color: #F3F3F3;
  color: #2D2D2D;
  border: none;
  padding: 8px; 
  width: 100%;
  height: 50px; 
  box-sizing: border-box;
}

.inputform input::placeholder {
  color: #797979;
}

.inputform .inputSubmit {
  font-size: 18px; 
  background-color: black;
  color: white;
  border: none;
  cursor: pointer;
  width: 150px;
  height: 60px; 
  display: flex;
  justify-content: center;
  align-items: center;
  text-transform: capitalize;
}
</style>
