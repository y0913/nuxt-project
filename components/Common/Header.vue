<template>
  <div>
    <v-app-bar
      class="header"
      app
      flat
      color="#FFFFFF"
      dark
      height="70"
      width="100%"
    >
    <v-container style="max-width: 1000px">
      <v-row>
        <v-col cols="6" align="left">
          <v-btn
            text
            plain
            :to="root"
            color="black"
          >
          {{title}}
          </v-btn>
        </v-col>
        <v-col
          cols="6"
          align="right"
        >
        <div class="btn-container">
          <v-btn
            v-for="(menu,i) in menus"
            :key="i"
            text
            color="red"
            :to="menu.root"
          >
            {{menu.name}}
          </v-btn>
        </div>
        </v-col>
      </v-row>
    </v-container>

    </v-app-bar>
  </div>
</template>

<script>

export default {
  name: 'Header',
  data () {
    return {
      menus:[
        {
          root:"About",
          name:"About Team"
        },
        {
          root:"Players",
          name:"Players"
        },
        {
          root:"Join",
          name:"Join Team?"
        },
      ],
      drawer: false,
      dialog: false,
      title: '京都フルカウンツ',
      root: '/'
    }
  }
};
</script>
