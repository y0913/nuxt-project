<template>
  <v-app dark>
    <Header />
    <v-main>
      <div style="margin: 0;">
        <Nuxt />
      </div>
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
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
