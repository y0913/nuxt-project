<template>
  <div class="players">
    <div class="headline font-weight-bold">{{ title }}</div>
    <div><span class="under">{{ titleJp }}</span></div>
    <v-row
      class="fill-height"
      align="center"
      justify="center"
    >
      <v-col class="d-flex justify-center scroll">
          <v-card
            class="mx-auto my-12 scroll"
            max-width="374"
            :to="{
              name: 'players-id',
              params: {
                id: 1
              }
            }"
          >
              <template slot="progress">
                <v-progress-linear
                  color="deep-purple"
                  height="10"
                  indeterminate
                ></v-progress-linear>
              </template>
            <v-img
              :src="umami"
              class="white--text align-end"
              height="250"
              cover
            >
            </v-img>
            <v-card-title>うまみ</v-card-title>
            <v-card-text>
              <v-row
                align="center"
                class="mx-0"
              >
              <div>ここに説明を書く ここに説明を書く ここに説明を書く ここに説明を書く</div>
              </v-row>
            </v-card-text>
          </v-card>
          <v-card
            class="mx-auto my-12 scroll"
            max-width="374"
            :to="{
              name: 'players-id',
              params: {
                id: 1
              }
            }"
          >
              <template slot="progress">
                <v-progress-linear
                  color="deep-purple"
                  height="10"
                  indeterminate
                ></v-progress-linear>
              </template>
            <v-img
              :src="kouno"
              class="white--text align-end"
              height="250"
              cover
            >
            </v-img>
            <v-card-title>こうの</v-card-title>
            <v-card-text>
              <v-row
                align="center"
                class="mx-0"
              >
              <div>ここに説明を書く ここに説明を書く ここに説明を書く ここに説明を書く</div>
              </v-row>
            </v-card-text>
          </v-card>
          <v-card
            class="mx-auto my-12 scroll"
            max-width="374"
            :to="{
              name: 'players-id',
              params: {
                id: 1
              }
            }"
          >
              <template slot="progress">
                <v-progress-linear
                  color="deep-purple"
                  height="10"
                  indeterminate
                ></v-progress-linear>
              </template>
            <v-img
              :src="hashimoto"
              class="white--text align-end"
              height="250"
              cover
            >
            </v-img>
            <v-card-title>レイカーズ</v-card-title>
            <v-card-text>
              <v-row
                align="center"
                class="mx-0"
              >
              <div>ここに説明を書く ここに説明を書く ここに説明を書く ここに説明を書く</div>
              </v-row>
            </v-card-text>
          </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import hashimoto from '../../assets/images/players/hashimoto.JPG'
import kouno from '../../assets/images/players/kouno.JPG'
import umami from '../../assets/images/players/umami.JPG'
export default {
  name: 'Players',
  data () {
    return {
      title: "PICK UP PLAYERS",
      titleJp: '注目選手',
      umami: umami,
      kouno: kouno,
      hashimoto: hashimoto
    }
  }
}
</script>

<style scoped lang="scss">
.under {
  border-bottom: solid 2px red;
}
.scroll {
  overflow-x: scroll;
}
</style>
