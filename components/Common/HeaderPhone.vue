<template>
  <v-container>
    <v-app-bar
      class="header"
      app
      flat
      color="#FFFFFF"
      dark
      elevate-on-scroll
    >
      <v-app-bar-nav-icon
        style="color: black;"
        @click="drawer = true"
        >
      </v-app-bar-nav-icon>

      <v-toolbar-title
        style="color: black;"
        class="font-weight-bold text-center"
        >
        {{title}}
      </v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
      fixed
      :clipped="false"
      app
    >
      <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Account</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </v-container>
</template>

<script>

export default {
  name: 'HeaderPhone',
  data () {
    return {
      menus:[
        {
          root:"about",
          name:"About"
        },
        {
          root:"players",
          name:"Players"
        },
        {
          root:"join",
          name:"Join Team?"
        },
      ],
      drawer: false,
      group: null,
      title: 'Kyoto Fullcounts',
      root: '/'
    }
  }
};
</script>
