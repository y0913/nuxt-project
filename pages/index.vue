<template>
  <div>
    <topPhone v-if="isSmartphone()"/>
    <topPc v-else />
  </div>
</template>

<script>
import topPc from '@/components/_pages/pc/top.vue'
import topPhone from '@/components/_pages/smartphone/topSm.vue'

export default {
  name: 'top',
  components: {
    topPc,
    topPhone
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
