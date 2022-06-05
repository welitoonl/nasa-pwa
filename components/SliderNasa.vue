<script>
  export default {
    data() {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
  }
</script>
<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="5000"
      controls
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <b-carousel-slide img-src="https://conteudo.imguol.com.br/c/entretenimento/1f/2020/07/17/nasa-pre-habilitacao-1595008254000_v2_900x506.jpg.webp"></b-carousel-slide>
      <b-carousel-slide img-src="https://static.poder360.com.br/2021/10/artemis-nasa.jpg"></b-carousel-slide>
      <b-carousel-slide img-src="https://www.unicesumar.edu.br/wp-content/uploads/2020/09/NASA-SPACE-APPS-e1601391131131.jpg"></b-carousel-slide>
    </b-carousel>
  </div>
</template>
