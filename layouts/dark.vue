<template>
  <v-app id="inspire">
    <!-- <v-app-bar color="transparent" app clipped-left>
      <v-toolbar-title>SAGALA</v-toolbar-title>
    </v-app-bar> -->
    <v-app-bar id="appbar" color="transparent" fixed no-gutters>
      <v-icon size="40">mdi-menu</v-icon>
      <v-spacer />
      <v-img
        id="logo_mobile"
        class="mx-2"
        :src="require('@/assets/logo.png')"
        max-height="40"
        max-width="40"
        contain
      ></v-img>
    </v-app-bar>
    <v-content>
      <v-container class="ma-0" pa-0 fill-height fluid>
        <nuxt-link to="/">
          <img id="logo" src="~assets/logo.png" />
        </nuxt-link>
        <nuxt />
      </v-container>
    </v-content>

    <v-footer id="footer_id" color="transparent" fixed padless>
      <v-row class="my-6" justify="end" no-gutters>
        <v-btn id="footers" color="white" text class="my-2 ml-4">
          SAGALA
        </v-btn>
        <v-spacer />
        <v-btn to="about" color="white" text class="my-2 mr-8">
          ABOUT US
        </v-btn>
        <v-btn
          href="http://instagram.com/sagala___"
          color="white"
          text
          class="my-2 mr-8"
        >
          INSTAGRAM
        </v-btn>
        <v-btn to="contact" color="white" text class="my-2 mr-8">
          CONTACT
        </v-btn>
      </v-row>
    </v-footer>
  </v-app>
</template>
<style scoped>
#appbar {
  display: none;
}
#logo {
  position: absolute;
  top: 0;
  right: 0%;
  max-width: 50%;
  width: 7%;
  margin: 20px;
  padding: 28px;
}
@media screen and (max-width: 768px) {
  #footer_id {
    display: none;
  }
  #logo {
    /* position: absolute;
    top: 0;
    right: 0%;
    max-width: 50%;
    width: 75px;
    margin: 10px;
    padding: 18px; */
    display: none;
  }
  #appbar {
    display: block;
  }
}
#persist {
  position: fixed;
  font-weight: 600;
  color: white;
  font-size: 50px;
  top: 40%;
  left: 17%;
  -webkit-font-smoothing: antialiased;
}
#footers {
  font-size: 31px;
}
#child {
  font-size: 13px;
}
@media screen and (max-width: 768px) {
  #persist {
    top: 40%;
    left: 16%;
    font-size: 18px;
  }
  #footers {
    font-size: 21px;
  }
}
</style>
<script>
export default {
  data: () => ({
    links: ['ABOUT US', 'INSTAGRAM', 'CONTACT'],
    logos: ['SAGALA']
  }),
  created() {
    this.$vuetify.theme.dark = true
  }
}
</script>
