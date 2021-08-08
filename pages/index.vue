<template>
  <div class="top">
    <div class="slider">
      <Carousel />
    </div>
    <div class="about">
      <About />
    </div>
    <div class="players">
      <Players />
    </div>
  </div>
</template>

<script>
import Carousel from '~/components/top/Carousel.vue'
import About from '~/components/top/About.vue'
import Players from '~/components/top/Players.vue'
export default {
  name: 'App',
  components: {
   Carousel,
   About,
   Players
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

<style scoped lang="scss">
  .top {
    margin: 0;
    padding: 0;
  }
</style>
