<template>
  <div class="text">
    <Carousel />
  </div>
</template>

<script>
import Carousel from '~/components/Common/Carousel.vue'
export default {
  name: 'App',
  components: {
   Carousel
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
