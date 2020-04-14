<template>
  <v-container id="layer" class="container" fluid>
    <img id="logo" class="ma-5 pa-7" src="~assets/logo.png" />
  </v-container>
</template>

<style scoped>
#layer {
  background: url('~assets/layer.png');
  background-size: cover;
}
#logo {
  position: absolute;
  top: 0;
  right: 0%;
  max-width: 50%;
  width: 7%;
}
#logo_bottom {
  position: relative;
  top: 0;
  right: 0%;
}
</style>
