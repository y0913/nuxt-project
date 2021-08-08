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
          <router-link to='/'>
            <div class="top">{{title}}</div>
          </router-link>
        </v-col>
        <v-col
          cols="6"
          align="right"
        >
          <v-menu offset-y>
            <template v-slot:activator="{on}">
              <v-btn
                class="mt-1"
                color="#ffffff"
                text
                height=40
                width=40
                v-on="on"
              >
                <v-avatar
                  v-if="userImage"
                  size=40
                  color="#ffffff"
                >
                <!-- ある場合とない場合で分ける -->
                  <v-icon dark>mdi-account-circle</v-icon>
                  <!-- <img :src="userImage"> -->
                </v-avatar>
            </v-btn>
            </template>
          </v-menu>
        </v-col>
      </v-row>
    </v-container>

    </v-app-bar>
  </div>
</template>

<script>

export default {
  name: 'App',
  data () {
    return {
      menus:[
        {root:"/mypage", name:"マイページ"},
        {root:"/account", name:"アカウント情報"},
      ],
      drawer: false,
      dialog: false,
      title: '京都フルカウンツ'
    }
  }
};
</script>
