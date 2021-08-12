<template>
  <v-container>
    <div class="ma-10">
      <div class="headline font-weight-bold">ABOUT KYOTO FULLCOUNTS</div>
      <div><span class="under">京都フルカウンツとは</span></div>
    </div>
    <div class="hero">
      <v-img
        :src="top"
        class="white--text align-end"
        height="600"
        >
        </v-img>
    </div>
  </v-container>
</template>

<script>
import top from '../../assets/images/top/top.JPG'
export default {
  name: 'About',
  data () {
    return {
      top: top
    }
  }
}
</script>

<style scoped lang="scss">
.under {
  border-bottom: solid 2px red;
}
</style>
