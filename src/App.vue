<script>
import Header from './components/Header.vue';
import Service from './components/Service.vue';
import Footer from './components/Footer.vue';
import LatestWork from './components/LatestWork.vue';
import Reviews from './components/Reviews.vue';


export default{
  components:{
    Header,Service, Footer, LatestWork, Reviews
  }
}
</script>

<template>
  <Header></Header>
  <Service></Service>
  <LatestWork></LatestWork>
  <Reviews></Reviews>
<Footer></Footer>

</template>

<style scoped>

</style>
