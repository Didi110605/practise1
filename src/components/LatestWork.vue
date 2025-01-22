<template>
  <div class="latestwork-wrapper">
    <h2 class="section-title">Latest work</h2>
    <div class="grid">
      <div v-for="item in latestwork" :key="item.id" class="grid-item">
        <img :src="item.image" class="latestwork-image" />
        <h3>{{ item.title }}</h3>
        <p>{{ item.text }}</p>
      </div>
    </div>
  </div>


</template>

<script>
export default{
  data(){
    return{
        latestwork: [ 
{id: 1, image: "/src/assets/Image.png", title: 'Project title', text: 'UI, Art drection'}, 
{id: 2, image: "/src/assets/Image (1).png", title: 'Project title', text: 'UI, Art drection'}, 
{id: 3, image: "/src/assets/Image (2).png", title: 'Project title', text: 'UI, Art drection'}, 
{id: 4, image: "/src/assets/Image (3).png", title: 'Project title', text: 'UI, Art drection'}, 
{id: 5, image: "/src/assets/Image (4).png", title: 'Project title', text: 'UI, Art drection'}, 
{id: 6, image: "/src/assets/Image (5).png", title: 'Project title', text: 'UI, Art drection'}
]

    }

  }
}
</script>


<style scoped>
.latestwork-wrapper {
  text-align: center;
  margin: 0 auto;
  max-width: 1200px;
  padding: 20px;
}

.section-title {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 20px;
  font-family: 'Arial', sans-serif;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 20px;
}

.grid-item {
  text-align: left;
}

.grid-item h3 {
    font-size: 20px;
    font-family: 'Arial', sans-serif;

}

.grid-item p{
    font-size: 17px;
    font-family: 'Arial', sans-serif;

}

.latestwork-image {
  width: 100%;
  height: auto;
  margin-bottom: 10px;
}
</style>
