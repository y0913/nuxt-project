<template>
  <v-container>
    <v-app-bar
      class="header"
      app
      flat
      color="#FFFFFF"
      dark
      hide-on-scroll
    >
      <v-toolbar-title
        style="color: black;"
        >
        <v-btn
          text
          plain
          :to="root"
          color="black"
          class="font-weight-bold text-center"
          style="font-size: 1.0em;"
        >
          {{title}}
        </v-btn>
      </v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      absolute
      top
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
          root:"/about",
          name:"About"
        },
        {
          root:"/players",
          name:"Players"
        },
        {
          root:"/join",
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
