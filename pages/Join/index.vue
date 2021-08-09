<template>
  <div class="hero">
    <div class="headline font-weight-bold">
      {{title}}
    </div>
    <v-card>
      <v-img
        :src="top"
        class="white--text align-end"
        height="600"
        >
        </v-img>
            <v-card-title>京都フルカウンツでは共に戦ってくれる仲間を募集しています。</v-card-title>
            <v-card-text>
              <v-row
                align="center"
                class="mx-0"
              >
              <div>ここに説明を書く ここに説明を書く ここに説明を書く ここに説明を書く</div>
              </v-row>
            </v-card-text>
      </v-card>
  </div>
</template>
<script>
import top from '../../assets/images/top/top.JPG'

export default {
  name: 'Players',
  data () {
    return {
      title: "選手募集",
      top: top,
    }
  }
}
</script>
