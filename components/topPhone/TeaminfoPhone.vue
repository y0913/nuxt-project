<template>
  <div class="teaminfo pa-5">
    <div class="headline font-weight-bold">{{ title }}</div>
    <div><span class="under">{{ titleJp }}</span></div>
    <v-row
      class="fill-height"
      align="center"
      justify="center"
    >
      <v-col class="d-flex scroll">
        <v-card
          class="mx-auto my-12 scroll-item pa-3"
          max-width="374"
          :to="{
            name: 'message'
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
            src="https://cdn.vuetifyjs.com/images/cards/house.jpg"
            class="white--text align-end"
            height="250"
          >
          </v-img>
          <v-card-title>{{derectorTitle}}</v-card-title>
          <v-card-text>
            <v-row
              align="center"
              class="mx-0"
            >
            <div>ここに説明を書く<br /> ここに説明を書く<br /> ここに説明を書く<br /> ここに説明を書く<br /></div>
            </v-row>
          </v-card-text>
        </v-card>

        <v-card
          class="mx-auto my-12 scroll-item pa-3"
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
            src="https://cdn.vuetifyjs.com/images/cards/house.jpg"
            class="white--text align-end"
            height="250"
          >
          </v-img>
          <v-card-title>{{staffTitle}}</v-card-title>
          <v-card-text>
            <v-row
              align="center"
              class="mx-0"
            >
            <div>ここに説明を書く<br /> ここに説明を書く<br /> ここに説明を書く<br /> ここに説明を書く<br /></div>
            </v-row>
          </v-card-text>
        </v-card>

        <v-card
          class="mx-auto my-12 scroll-item pa-3"
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
            src="https://cdn.vuetifyjs.com/images/cards/house.jpg"
            class="white--text align-end"
            height="250"
          >
          </v-img>
          <v-card-title>{{otherTitle}}</v-card-title>
          <v-card-text>
            <v-row
              align="center"
              class="mx-0"
            >
            <div>ここに説明を書く<br /> ここに説明を書く<br /> ここに説明を書く<br /> ここに説明を書く<br /></div>
            </v-row>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'Teaminfo',
  data () {
    return {
      derectorTitle: "監督メッセージ",
      staffTitle: "スタッフメッセージ",
      otherTitle: "選手一覧ページ",
      title: "TEAM INFO",
      titleJp: "チーム情報",
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
  .scroll-item {
    flex: 0 0 auto;
  }
}
</style>
