<template>
<carousel>
  <carousel-slide>
    <div style="position:absolute; left:0; right:0; text-align:center; top:50%; color:#fff; font-size:16px,">Salut les gens</div>
    <img src="http://lorempicsum.com/futurama/630/300/1" width=100%>
  </carousel-slide>
  <carousel-slide>
    <div style="position:absolute; left:0; right:0; text-align:center; top:50%; color:#fff; font-size:16px,">Au revoir les gens</div>
    <img src="http://lorempicsum.com/futurama/630/300/2" width=100%>
  </carousel-slide>
</carousel>
</template>

<script>

import Carousel from './components/carousel/Carousel'
import CarouselSlide from './components/carousel/CarouselSlide'
export default {
  name: 'app',
  components: {
    Carousel,
    CarouselSlide
  }
}
</script>
