<template>
  <div class="about">
    <div class="headline font-weight-medium text-center">{{ title }}</div>
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
            <div>ここに説明を書く ここに説明を書く ここに説明を書く ここに説明を書く</div>
            </v-row>
          </v-card-text>
          <v-card-actions>
            <v-btn
              color="deep-purple lighten-2"
              text
              @click="details"
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
            <div>ここに説明を書く ここに説明を書く ここに説明を書く ここに説明を書く</div>
            </v-row>
          </v-card-text>
          <v-card-actions>
            <v-btn
              color="deep-purple lighten-2"
              text
              @click="details"
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
            <div>ここに説明を書く ここに説明を書く ここに説明を書く ここに説明を書く</div>
            </v-row>
          </v-card-text>
          <v-card-actions>
            <v-btn
              color="deep-purple lighten-2"
              text
              @click="details"
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
export default {
  name: 'About',
  data () {
    return {
      derectorTitle: "監督メッセージ",
      staffTitle: "スタッフメッセージ",
      otherTitle: "選手一覧ページ",
      title: "チーム情報"
    }
  }
}
</script>
