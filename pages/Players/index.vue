<template>
<div class="players">
  <div class="hero">
  <div class="ma-10">
    <div class="headline font-weight-bold">PLAYERS</div>
    <div><span class="under">フルカウンツの主役たち</span></div>
  </div>
    <v-img
      :src="top"
      class="white--text align-end"
      height="600"
      >
      </v-img>
  </div>
  <div class="headline font-weight-medium text-center mt-10">{{ title }}</div>
      <v-row
      class="fill-height"
      align="center"
      justify="center"
    >
      <v-col class="d-flex justify-center" justify="center" align-content="center">
          <v-card
            class="mx-auto my-12"
            max-width="374"
          >
              <template slot="progress">
                <v-progress-linear
                  color="deep-purple"
                  height="10"
                  indeterminate
                ></v-progress-linear>
              </template>
            <v-img
              :src="catcher"
              class="white--text align-end"
              height="250"
            >
            </v-img>
            <v-card-title>タイトル考える</v-card-title>
            <v-card-text>
              <v-row
                align="center"
                class="mx-0"
              >
              <div>ここに説明を書く ここに説明を書く ここに説明を書く ここに説明を書く</div>
              </v-row>
            </v-card-text>
            <v-card-actions>
              <v-btn
                color="deep-purple lighten-2"
                text
              >
                詳細
              </v-btn>
            </v-card-actions>
          </v-card>

          <v-card
            class="mx-auto my-12"
            max-width="374"
          >
              <template slot="progress">
                <v-progress-linear
                  color="deep-purple"
                  height="10"
                  indeterminate
                ></v-progress-linear>
              </template>
            <v-img
              :src="catcher"
              class="white--text align-end"
              height="250"
            >
            </v-img>
            <v-card-title>タイトル考える</v-card-title>
            <v-card-text>
              <v-row
                align="center"
                class="mx-0"
              >
              <div>ここに説明を書く ここに説明を書く ここに説明を書く ここに説明を書く</div>
              </v-row>
            </v-card-text>
            <v-card-actions>
              <v-btn
                color="deep-purple lighten-2"
                text
              >
                詳細
              </v-btn>
            </v-card-actions>
          </v-card>

          <v-card
            class="mx-auto my-12"
            max-width="374"
          >
              <template slot="progress">
                <v-progress-linear
                  color="deep-purple"
                  height="10"
                  indeterminate
                ></v-progress-linear>
              </template>
            <v-img
              :src="catcher"
              class="white--text align-end"
              height="250"
            >
            </v-img>
            <v-card-title>タイトル考える</v-card-title>
            <v-card-text>
              <v-row
                align="center"
                class="mx-0"
              >
              <div>ここに説明を書く ここに説明を書く ここに説明を書く ここに説明を書く</div>
              </v-row>
            </v-card-text>
            <v-card-actions>
              <v-btn
                color="deep-purple lighten-2"
                text
              >
                詳細
              </v-btn>
            </v-card-actions>
          </v-card>
      </v-col>
    </v-row>
</div>
</template>

<script>
import top from '../../assets/images/top/top.JPG'
import catcher from '../../assets/images/players/catcher.JPG'
export default {
  name: 'Players',
  data () {
    return {
      title: "選手一覧",
      top: top,
      catcher: catcher
    }
  }
}
</script>

<style scoped lang="scss">
.under {
  border-bottom: solid 2px red;
}
</style>
