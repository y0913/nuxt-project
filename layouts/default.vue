<template>
  <v-app dark>
    <HeaderPhone v-if="isSmartphone()" />
    <Header v-else/>
    <v-main>
      <!-- <div style="margin: 0;"> -->
      <v-container>
        <Nuxt />
      </v-container>
      <!-- </div> -->
    </v-main>
    <FooterPhone v-if="isSmartphone()" />
    <Footer v-else />
  </v-app>
</template>

<script>
import Header from '~/components/Common/Header.vue'
import HeaderPhone from '~/components/Common/HeaderPhone.vue'
import Footer from '~/components/Common/Footer.vue'
import FooterPhone from '~/components/Common/FooterPhone.vue'
export default {
  name: 'App',
  components: {
   Header,
   HeaderPhone,
   Footer,
   FooterPhone
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
  },
  methods: {
    isSmartphone() {
      return this.$ua.isFromSmartphone()
      }
  }
}
</script>
