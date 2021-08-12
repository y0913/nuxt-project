<template>
  <v-carousel
    class="carousel pb-5"
    cycle
    height="374"
    width="100%"
    hide-delimiters
    :show-arrows="false"
  >
    <v-carousel-item
      :src="top"
      cover
    >

    </v-carousel-item>
  </v-carousel>
</template>

<script>
import top from '../../assets/images/top/top.JPG'
export default {
  name: 'Carousel',
  data () {
    return {
      colors: [
        'indigo',
        'warning',
        'pink darken-2',
        'red lighten-1',
        'deep-purple accent-4',
      ],
      slides: [
        'First',
        'Second',
        'Third',
        'Fourth',
        'Fifth',
      ],
      top: top
    }
  }
}
</script>
