<template>
  <div class="top">
    <div class="slider">
      <Carousel />
    </div>
    <div class="about">
      <About />
    </div>
  </div>
</template>

<script>
import Carousel from '~/components/top/Carousel.vue'
import About from '~/components/top/About.vue'
export default {
  name: 'App',
  components: {
   Carousel,
   About
  },
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      miniVariant: false,
      right: true,
      rightDrawer: false,
    }
  }
}
</script>
