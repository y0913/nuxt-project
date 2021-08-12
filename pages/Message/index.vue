<template>
  <v-container>
    <div class="ma-10">
      <div class="headline font-weight-bold">{{ title }}</div>
      <div><span class="under">監督メッセージ</span></div>
    </div>
    <v-row
      class="fill-height"
      align="center"
      justify="center"
    >
      <v-col cols=6>
        <v-img
          :src="derector"
          height="600"
          contain
        ></v-img>
      </v-col>
      <v-col cols=6>
        <div class="message">
          監督の小澤です。
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
          なんかメッセージを考えてもらう。<br />
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
import derector from '../../assets/images/players/derector.JPG'
export default {
  name: 'message',
  data() {
    return {
      title: 'MESSAGE',
      derector: derector
    }
  }
}
</script>

<style scoped lang="scss">
.under {
  border-bottom: solid 2px red;
}
</style>
