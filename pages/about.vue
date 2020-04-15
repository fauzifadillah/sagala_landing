/* eslint-disable prettier/prettier */ /* eslint-disable prettier/prettier */
<template>
  <v-container id="layer" class="container ma-0 pa-0" fill-height fluid>
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
        SAGALA, is a creative technology company in Bandung since 2020.<br />
        Our Vision is improving businesses through the collaboration of
        Technology and Creativity<br /><br />We provide 3 main solutions:
        <br /><br />
        First, The TechSol (Technology-based Solution), such as: Data Discovery,
        IoT Platform, Full-Stack Application Development, End-to-End E-Commerce
        Development, POS Platform (Point of Sale). <br /><br />
        Second, The C&D (Creative and Design Solution) such as: Branding
        activation (marketing kit), Social media activation (content), Company
        profile, Event documentary, Product campaign, Web design.<br /><br />
        Third, The Strategic Planning Creative and Event Solution, such as:
        Event production and Running event. <br /><br />
        We believe, with the power of technology and creativity, we can solve
        all of your business problem in just a solution.
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
    <v-col id="abt" cols="12" lg="6" justify="center" align="center">
      <img :src="require(`../assets/about.png`)" />
    </v-col>
  </v-container>
</template>
<style scoped>
@media screen and (max-width: 768px) {
  #abt img {
    height: 200px;
    box-sizing: border-box;
    max-width: 100%;
    max-height: 100%;
    width: 200px;
  }

  p {
    font-size: 14px;
    margin: 0px;
  }

  #head {
    margin-right: 48px;
  }
}
#head {
  justify-items: center;
  align-items: center;
}
#layer {
  background: url('~assets/layer.png');
  background-size: cover;
}
</style>
<script>
export default {
  layout: 'dark'
}
</script>
