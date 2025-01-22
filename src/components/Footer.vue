<template>
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

<script>
export default{

}
</script>

<style scoped>
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