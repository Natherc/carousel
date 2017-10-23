<template>
  <div id="app">
    <carousel>
      <carousel-slide>YO</carousel-slide>
       <carousel-slide>YA</carousel-slide>

    </carousel>
  </div>
</template>

<script>
import carousel from './components/carousel/Carousel'
import carouselSlide from './components/carousel/CarouselSlide'


export default {
  name: 'app',
  components: {
    carousel,
    carouselSlide,
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
