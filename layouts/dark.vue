<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      fixed
      app
      width="512"
      color="transparent"
      :src="require('@/assets/layer.jpg')"
      justify="center"
      align="center"
    >
      <v-img
        id="logo_mobile"
        class="mx-2"
        :src="require('@/assets/spacer.png')"
        height="75"
        width="1px"
        contain
      ></v-img>
      <v-btn id="x" color="white" text rounded @click.stop="drawer = !drawer">
        <v-icon>mdi-close-thick</v-icon>
      </v-btn>
      <v-list justify="center" align="center" style="align-items:'center'">
        <v-list-item to="/" router exact justify="center" align="center">
          <v-list-item-content justify="center" align="center">
            <v-list-item-title style="font-size: 40px;">HOME</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item to="/about" router exact justify="center" align="center">
          <v-list-item-content justify="center" align="center">
            <v-list-item-title style="font-size: 40px;"
              >ABOUT</v-list-item-title
            >
          </v-list-item-content>
        </v-list-item>
        <v-list-item
          href="http://instagram.com/sagala___"
          router
          exact
          justify="center"
          align="center"
        >
          <v-list-item-content justify="center" align="center">
            <v-list-item-title style="font-size: 40px;"
              >INSTAGRAM</v-list-item-title
            >
          </v-list-item-content>
        </v-list-item>
        <v-list-item to="/contact" router exact justify="center" align="center">
          <v-list-item-content justify="center" align="center">
            <v-list-item-title style="font-size: 40px;"
              >CONTACT</v-list-item-title
            >
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      id="appbar"
      color="transparent"
      fixed
      no-gutters
      @click.stop="drawer = !drawer"
    >
      <v-icon size="40">mdi-menu</v-icon>
      <v-spacer />
      <v-img
        id="logo_mobile"
        class="mx-2"
        :src="require('@/assets/logo.png')"
        max-height="25"
        max-width="25"
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
        <v-btn
          id="footers"
          href="http://sagalagroup.com"
          color="white"
          text
          class="my-2 ml-4"
        >
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
#logomb {
  position: fixed;
  font-weight: 600;
  color: white;
  font-size: 50px;
  top: 40%;
  left: 17%;
  -webkit-font-smoothing: antialiased;
  display: none;
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
  #logomb {
    position: fixed;
    font-weight: 600;
    color: white;
    font-size: 50px;
    top: 40%;
    left: 12%;
    -webkit-font-smoothing: antialiased;
    display: block;
  }
  #footers {
    font-size: 21px;
  }
}
</style>
<script>
export default {
  data: () => ({
    logo: require('@/assets/logo.png'),
    drawer: false,
    items: [
      {
        icon: '',
        title: 'HOME',
        to: '/'
      },
      {
        icon: '',
        title: 'ABOUT',
        to: '/about'
      },

      {
        icon: '',
        title: 'INSTAGRAM',
        to: 'http://instagram.com/sagala___'
      },
      {
        icon: '',
        title: 'CONTACT',
        to: '/contact'
      }
    ]
  }),
  created() {
    this.$vuetify.theme.dark = true
  }
}
</script>
