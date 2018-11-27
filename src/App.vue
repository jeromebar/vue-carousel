<template>
  <div>
    <carousel>
      <carousel-slide v-for="n in slides" :index="n - 1">
        <div style="position:absolute; left:0; right:0; text-align:center; top:50%; color:#fff; font-size:16px,">Slides
          {{n}}
        </div>
        <img :src="`http://lorempicsum.com/futurama/630/300/${n}`" width=100%>
      </carousel-slide>
    </carousel>
    <button @click="addSlide">Ajouter un slide</button>
    <button @click="removeSlide">Supprimer un slide</button>
  </div>
</template>

<script>

  import Carousel from './components/carousel/Carousel'
  import CarouselSlide from './components/carousel/CarouselSlide'

  export default {
    data() {
      return {
        name: 'app',
        slides: 5
      }
    },
    methods: {
      addSlide() {
        this.slides++
      },
      removeSlide() {
        this.slides--
      }
    },
    components: {
      Carousel,
      CarouselSlide
    }
  }
</script>
