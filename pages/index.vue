<template>
  <div>
    <!-- <topPhone v-if="isSmartphone()"/> -->
    <topPc />
  </div>
</template>

<script>
import topPc from '@/components/_pages/pc/top.vue'

export default {
  name: 'top',
  components: {
    topPc
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
  },
  methods: {
    isSmartphone(){
      return this.$ua.isFromSmartphone()
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
