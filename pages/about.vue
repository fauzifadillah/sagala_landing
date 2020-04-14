<template>
  <v-row id="port2" justify="start" align="start" fill-height fluid>
    <v-col id="head" cols="12" lg="6">
      <div style="text-align:left;">
        <img
          justify="start"
          align="start"
          class="pa-4 ml-12"
          :src="require(`../assets/abouthead.png`)"
        />
      </div>
      <p justify="start" align="start" class="display-2 ma-1 pa-4 ml-12">
        / ABOUT US
      </p>
      <p justify="start" align="start" class="text-lg ma-1 pa-4 ml-12">
        / SAGALA, a technology-based creative industry company in Bandung
        especially in information and design systems was founded in 2020. We
        have 3 main divisions, namely the Technology Division which consists of:
        Big Data Analytics, IOT Platform, Full-Pack Application Development,
        Security Penetration Services, End - to - End E - Commerce development,
        Control and Monitoring systems, Laboratory Management Systems, POA
        Platform (Point of Sale), Creative and Design Division and Strategic
        Planning Creative and Event. Sagala emerged based on creativity and
        technology aimed at developing the technology-based creative industry
        sector. We believe, by using technology and creativity to the maximum
        level, it will maximize your business. Sagala will be ready to serve
        your business and creative things to produce creativity based on
        technology.
      </p>
      <div style="text-align:left;">
        <img
          justify="start"
          align="start"
          class="pa-4 ml-12"
          :src="require(`../assets/abouthead.png`)"
        />
      </div>
    </v-col>
    <v-col cols="12" lg="6" justify="center" align="center">
      <img :src="require(`../assets/about.png`)" />
    </v-col>
  </v-row>
</template>
<style scoped>
#head {
  justify-items: center;
  align-items: center;
}
</style>
<script>
export default {
  layout: 'dark'
}
</script>
