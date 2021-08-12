<template>
<v-container>
    <div class="mb-10">
      <div class="headline font-weight-bold">{{ title }}</div>
      <div><span class="under">{{ titleJp }}</span></div>
    </div>
    <v-card
      class="mx-auto"
      color="#26c6da"
    >
      <v-card-title class="text-h5">
        <v-icon
        large
        left
        color="white"
        >mdi-twitter</v-icon>
        <span class="font-weight-light" style="color: white;">Twitter</span>
      </v-card-title>
      <v-card-text>
        <a class="twitter-timeline" data-height="600" href="https://twitter.com/fullcounts2015?ref_src=twsrc%5Etfw">Tweets by fullcounts2015</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
      </v-card-text>
    </v-card>
  </v-container>
</template>

<script>
  export default {
    name: 'News',
    data() {
      return {
        title: 'LATEST NEWS',
        titleJp: '最新情報',
      }
    },
  }
</script>

<style scoped lang="scss">
.under {
  border-bottom: solid 2px red;
}
</style>
