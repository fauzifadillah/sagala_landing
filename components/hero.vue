<template>
  <v-container id="layer" class="container" fluid>
    <nuxt-link to="/">
      <img id="logo" src="~assets/logo.png" />
    </nuxt-link>
  </v-container>
</template>

<style scoped>
#layer {
  background: url('~assets/layer.jpg');
  background-size: cover;
}
#logo {
  position: absolute;
  margin: 20px;
  padding: 28px;
  top: 0;
  right: 0%;
  max-width: 50%;
  width: 7%;
}

@media screen and (max-width: 768px) {
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
}
#logo_bottom {
  position: relative;
  top: 0;
  right: 0%;
}
</style>
