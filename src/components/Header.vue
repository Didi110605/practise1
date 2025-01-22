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
        <p class="text3">
          This is a template Figma file, turned into code using Anima.
          <br />
          Learn more at AnimaApp.com
        </p>
        <button class="button">Contact</button>
      </div>
      <img :src="image" class="image" />
    </div>
    <div class="logosWraper">
      <img :src="imgGoogle" />
      <img :src="imgNike" />
      <img :src="imgSamsung" />
      <img :src="imgApple" />
      <img :src="imgAdidas" />
    </div>
  </template>
  
  <script>
  import image from "../assets/girl.png";
  import imgGoogle from "../assets/logogoogle.png";
  import imgNike from "../assets/logonike.png";
  import imgSamsung from "../assets/logosamsung.png";
  import imgApple from "../assets/logoApple.png";
  import imgAdidas from "../assets/logoadidas.png";
  
  export default {
    name: "Header",
    data() {
      return {
        image,
        imgGoogle,
        imgNike,
        imgSamsung,
        imgApple,
        imgAdidas,
      };
    },
  };
  </script>
  

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
    margin-top: 40px; 
  margin-bottom: 20px; 
    height: auto;
    display: flex;
    justify-content: space-between;
    padding: 10px;
    img{
      height: 100%;
    }

  }
</style>