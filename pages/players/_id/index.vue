<template>
  <v-card flat class="d-inline-block mx-auto">
    <v-container>
      <v-row  justify="space-between">
        <v-col>
          <v-card-title class="pl-0">Fullcounts #22: 近藤</v-card-title>
          <v-img
            :src="catcher"
            class="white--text align-end"
            height="500"
          ></v-img>
        </v-col>
        <v-col>
          <p>名前: 近藤</p>
        </v-col>
      </v-row>
    </v-container>
  </v-card>
</template>

<script>
import top from '~/assets/images/top/top.JPG'
import catcher from '~/assets/images/players/catcher.JPG'
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
