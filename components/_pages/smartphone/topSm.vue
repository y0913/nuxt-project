<template>
  <div class="top">
    <div class="mb-10">
      <Carousel />
    </div>
    <div class="mb-10">
      <About />
    </div>
    <div class="mb-10">
      <Players />
    </div>
    <!-- <div class="mb-10">
      <Teaminfo />
    </div> -->
    <div class="mb-10">
      <News />
    </div>
  </div>
</template>

<script>
import Carousel from '~/components/topPhone/CarouselPhone.vue'
import About from '~/components/topPhone/AboutPhone.vue'
import Players from '~/components/topPhone/PlayersPhone.vue'
import News from '~/components/top/News.vue'
import Teaminfo from '~/components/topPhone/TeaminfoPhone.vue'

export default {
  name: 'topPc',
  components: {
   Carousel,
   About,
   Players,
   News,
   Teaminfo
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
