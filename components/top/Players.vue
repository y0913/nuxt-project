<template>
  <div class="players">
    <v-row>
      <v-col>
        <v-card>
          <div class="d-flex justify-center">
            <v-img
              src="https://cdn.vuetifyjs.com/images/cards/plane.jpg"
              class="white--text align-end"
              height="600px"
            >
              <v-card-title>{{title}}</v-card-title>
            </v-img>
          </div>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'Players',
  data () {
    return {
      colors: [
        'indigo',
        'warning',
        'pink darken-2',
        'red lighten-1',
        'deep-purple accent-4',
      ],
      slides: [
        'First',
        'Second',
        'Third',
        'Fourth',
        'Fifth',
      ],
      title: "選手一覧"
    }
  }
}
</script>
