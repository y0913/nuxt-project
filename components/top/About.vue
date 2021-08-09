<template>
  <div class="about">
    <div class="headline font-weight-bold">{{ title }}</div>
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
      <v-col>
        <v-spacer></v-spacer>
        <v-btn
          color="deep-purple lighten-2"
          style="color: white;"
          align="right"
          justify="right"
          @click="details"
        >
          詳しく見る
        </v-btn>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import common from '../../assets/images/common/common.JPG'
export default {
  name: 'About',
  data () {
    return {
      derectorTitle: "監督メッセージ",
      staffTitle: "スタッフメッセージ",
      otherTitle: "選手一覧ページ",
      title: "About Us",
      common: common
    }
  }
}
</script>
