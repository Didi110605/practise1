<template>
   <div class="services-wrapper">
    <div class="service" v-for="item in services" :key="item.id">
      <img :src="item.image"  class="service-image" />
      <h3>{{ item.title }}</h3>
      <p>{{ item.text }}</p>
    </div>
  </div>


</template>

<script>
export default{
  data(){
    return{
        services: [ 
{id: 1, image: "/src/assets/Pink.png", title: 'Product Design', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}, 
{id: 2, image: "/src/assets/Orange.png", title: 'Visual Design', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'},
{id: 3, image: "/src/assets/Green.png", title: 'Art Direction', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}
]

    }

  }
}

</script>

<style scoped>
.services-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 80px 0;
}

.service {
  flex: 1;
  margin: 0 20px;
  text-align: center;
}

.service-image {
  width: 100px;
  height: 100px;
  object-fit: contain;
  margin-bottom: 20px;
}

.service h3 {
  font-weight: bold;
  font-family: 'Arial', sans-serif;
  font-size: 27px;
}

.service p {
  font-size: 17px;
  color: #555;
  font-family: 'Arial', sans-serif;

}


</style>