<template>
  <div class="reviews-section">
    <h1 class="reviews-title">Testimonial</h1>
    <div class="reviews-container">
      <div class="reviews" v-for="(item, id) in reviews" :key="id">
        <p class="review-text">{{ item.text }}</p>
        <div class="reviewer">
          <img :src="item.image" alt="User Image" class="reviewer-image" />
          <div>
            <div class="stars">
              <span v-for="star in 5" :key="star" class="star">&#9733;</span>
            </div>
            <h3>{{ item.name }}</h3>
            <p>{{ item.company }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>


</template>

<script>
export default {
  data() {
    return {
      reviews: [
        {id: 1,text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com",image: "/src/assets/Client Image.png",name: "Gemma Nolen",company: "Google" },
        {id: 2,text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com",image: "/src/assets/Client Image.png",name: "Gemma Nolen",company: "Google" },
        {id: 3,text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com",image: "/src/assets/Client Image.png",name: "Gemma Nolen",company: "Google" },
        {id: 4,text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com",image: "/src/assets/Client Image.png",name: "Gemma Nolen",company: "Google" },
        {id: 5,text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com",image: "/src/assets/Client Image.png",name: "Gemma Nolen",company: "Google" },
        {id: 6,text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com",image: "/src/assets/Client Image.png",name: "Gemma Nolen",company: "Google" },
      ]
    };
  }
};

</script>

<style scoped>
.reviews-section {
  text-align: center;
  padding: 20px;
  font-family: Arial, sans-serif;
}

.reviews-title {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 20px;
}

.reviews-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}

.reviews {
  background-color: #F3F3F3;
  border: 1px solid #eaeaea;
  width: 400px;
  height: 330px;
  padding: 20px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  text-align: left;
}

.review-text {
  font-size: 20px;
  line-height: 1.5;
  margin-bottom: 20px;
  color: #333333;
  text-align: center;
}

.reviewer {
  display: flex;
  align-items: center;
  gap: 10px;
}

.reviewer-image {
  border-radius: 50%;
  width: 50px;
  height: 50px;
  
}

.stars {
  display: flex;
}

.star {
  color: rgb(0, 0, 0);
  font-size: 16px;
}

.reviewer-item h3 {
  font-size: 20px;
  font-weight: bold;
  color: #000;
  font-family: 'Arial', sans-serif;
}

.reviewer-item p {
  font-size: 14px;
  color: #666666;
  font-family: 'Arial', sans-serif;
}


</style>