<template>
  <v-container id="layer" class="container ma-0 pa-0" fill-height fluid>
    <v-col id="head" cols="12">
      <img class="pa-4 ml-12" :src="require(`../assets/abouthead.png`)" />
      <p class="display-2 ma-1 pa-4 ml-12">/ CONTACT US</p>
      <p class="title ma-1 pa-4 ml-12">
        <v-icon class="my-auto mr-1 pa-1">mdi-phone</v-icon>+6285795752481
      </p>
      <p class="title ma-1 pa-4 ml-12">
        <v-icon class="my-auto mr-1 pa-1">mdi-email</v-icon
        >admin@sagalagroup.com
      </p>
      <p class="title ma-1 pa-4 ml-12">
        <v-icon class="my-auto mr-1 pa-1">mdi-instagram</v-icon>@sagala___
      </p>
      <p class="title ma-1 pa-4 ml-12">
        <v-icon class="my-auto mr-1 pa-1">mdi-map-marker</v-icon>Jl. Pratista
        Bar.VIII No.7A, Antapani Kidul Bandung Jawa Barat 40291
      </p>
    </v-col>
  </v-container>
</template>
<style scoped>
#layer {
  background: url('~assets/contact.png');
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
<script>
export default {
  layout: 'dark'
}
</script>
