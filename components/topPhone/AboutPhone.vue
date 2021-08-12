<template>
  <div class="about">
    <div class="headline font-weight-bold">{{ title }}</div>
    <div><span class="under">京都フルカウンツについて</span></div>
    <v-row
      class="fill-height"
      align="center"
      justify="center"
    >
      <v-col class="d-flex justify-center">
        京都フルカウンツは京都府野球連盟に所属する社会人野球のクラブチームです。
        <br />なんか色々書いていくー
        <br />なんか色々書いていくー
        <br />なんか色々書いていくー
        <br />なんか色々書いていくー
        <br />なんか色々書いていくー
        <br />なんか色々書いていくー
        <br />なんか色々書いていくー
      </v-col>
    </v-row>
    <v-row>
      <v-col class="d-flex justify-right">
        <v-spacer></v-spacer>
        <v-btn
          color="deep-purple lighten-2"
          style="color: white;"
          align="right"
          justify="right"
        >
          詳しく見る
        </v-btn>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'About',
  data () {
    return {
      title: "ABOUT TEAM",
    }
  }
}
</script>

<style scoped lang="scss">
.under {
  border-bottom: solid 2px red;
}
.scroll {
  overflow-x: auto;
}
</style>
