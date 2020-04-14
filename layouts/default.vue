<template>
  <v-app id="inspire">
    <!-- <v-app-bar color="transparent" app clipped-left>
      <v-toolbar-title>SAGALA</v-toolbar-title>
    </v-app-bar> -->

    <v-content>
      <v-container class="ma-0" pa-0 fluid>
        <nuxt />
        <h2 id="persist" class="subtitle">
          CREATIVE TECHNOLOGY
        </h2>
      </v-container>
    </v-content>

    <v-footer color="transparent" app padless>
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
<style>
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
