<template>
  <v-app dark>
    <Header />
    <v-main>
      <!-- <div style="margin: 0;"> -->
      <v-container>
        <Nuxt />
      </v-container>
      <!-- </div> -->
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import Header from '~/components/Common/Header.vue'
import Footer from '~/components/Common/Footer.vue'
export default {
  name: 'App',
  components: {
   Header,
   Footer
  },
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      miniVariant: false,
      right: true,
      rightDrawer: false,
    }
  }
}
</script>
