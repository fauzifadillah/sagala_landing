<template>
  <v-container class="container ma-0 pa-0" fill-height fluid>
    <hero />
    <!-- <porto /> -->
    <port gambar="claus" />
    <!-- <port gambar="port2" /> -->
    <!-- <port />
    <port />
    <port />
    <port />
    <port /> -->
    <v-footer color="transparent" class="text-center white--text" cols="12">
      <v-col
        color="transparent"
        class="text-lg text-center white--text"
        cols="12"
      >
        Copyright {{ new Date().getFullYear() }} &copy;
        <strong> SAGALAGROUP</strong>
      </v-col>
    </v-footer>
  </v-container>
</template>

<script>
import hero from '~/components/hero.vue'
import port from '~/components/port.vue'

export default {
  components: {
    hero,
    port
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  max-width: 100%;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
