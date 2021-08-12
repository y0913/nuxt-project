<template>
    <v-footer>
        <v-bottom-navigation
          sticky
          horizontal
          fixed
          :hide-on-scroll = "false"

        >
          <v-btn
            color="deep-purple accent-4"
            text
          >
            <span>ABOUT</span>
            <v-icon>mdi-debug-step-over</v-icon>
          </v-btn>

          <v-btn
            color="deep-purple accent-4"
            text
          >
            <span>PLAYERS</span>
            <v-icon>mdi-account-multiple</v-icon>
          </v-btn>

          <v-btn
            color="deep-purple accent-4"
            text
          >
            <span>JOIN</span>
            <v-icon>mdi-thumb-up</v-icon>
          </v-btn>
        </v-bottom-navigation>
    </v-footer>
</template>

<script>

export default {
  name: 'FooterPhone',
  data () {
    return {
      fixed: true,
    }
  }
};
</script>
