<template>
  <v-row id="main_port">
    <v-row justify="end" class="mr-10">
      <p class="headline ma-1 pa-4 ml-12">RECENT WORK</p>
    </v-row>
    <v-row id="port1">
      <v-col cols="6" md="4">
        <img :src="require(`../assets/port-1-1.jpg`)" />
      </v-col>
      <v-col cols="12" md="8">
        <img :src="require(`../assets/port-1-2.jpg`)" />
      </v-col>
    </v-row>
    <v-row id="port2">
      <v-col cols="6" md="4">
        <img :src="require(`../assets/port-2-1.jpg`)" />
      </v-col>
      <v-col cols="6" md="4">
        <img :src="require(`../assets/port-2-2.jpg`)" />
      </v-col>
      <v-col cols="6" md="4">
        <img :src="require(`../assets/port-2-3.jpg`)" />
      </v-col>
    </v-row>
    <v-row id="port3">
      <v-col cols="6" md="4">
        <img id="port3-1" :src="require(`../assets/port-3-1.jpg`)" />
      </v-col>
      <v-col class="pr-0" cols="12" md="8">
        <img id="port3-2" :src="require(`../assets/port-3-2.jpg`)" />
      </v-col>
    </v-row>
  </v-row>
</template>
<style scoped>
#main_port {
  /* background: url('~assets/layer.png'); */
  /* background-size: cover; */
}
#port1 img {
  object-fit: cover;
  max-width: 100%;
  height: 700px;
}
#port2 img {
  object-fit: cover;
  max-width: 100%;
  height: 700px;
}

#port3 img {
  object-fit: cover;
  max-width: 100%;
  /* height: 700px; */
}

#port3-1 {
  object-fit: cover;
  max-width: 100%;
  width: 100%;
  /* height: 750px; */
}

#port3-2 {
  object-fit: cover;
  max-width: 100%;
  width: 100%;
  /* width: fill; */
  /* height: 650px; */
}

#port4-1 {
  object-fit: cover;
  max-width: 100%;
  /* height: 750px; */
}
</style>
<script>
export default {
  props: {
    gambar: {
      default: 'claus',
      type: String,
      required: false
    }
  }
}
</script>
