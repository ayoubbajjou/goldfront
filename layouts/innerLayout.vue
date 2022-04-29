<template>
  <v-app id="app" light>
    <v-container class="background pa-0 ">
     <v-row>
        <v-col cols="12" lg="5" md="12" sm="12">
          <v-list class="mt-16" color="
          transparent">
          <v-list-item-title class=""><h2 class=" white--text text-right">MEIN GEIGER GOLDSPARPLAN</h2></v-list-item-title>
          <v-list-item-subtitle ><h2 class=" font-weight-light text-right text">
            Eine glänzende Idee für Ihre Zukunft!
          </h2></v-list-item-subtitle>
          </v-list>

        </v-col>
        <v-col cols="12" lg="2" md="12" sm="12">
          <v-img
            :src="require('../assets/Geiger-goldsparplan-goldbarren-50g.png')"
            width="100%"
            class="mt-16 headerImage"
          ></v-img>
        </v-col>
        <v-col cols="12" lg="5" md="12" sm="12">
          <v-img
            :src="
              require('../assets/Header.png' )
            "
            width="100%"

          ></v-img>
        </v-col>
      </v-row>

 <v-app-bar class="elevation-0 border" color="white">

        <h4 class="text-uppercase ml-16" @click="changeRoute('Ubersicht')"
        > Übersicht </h4>
        <h4 class="text-uppercase ml-6" @click="changeRoute('Umsatze')"> Umsatze </h4>

        <h4 class="text-uppercase ml-6" @click="changeRoute('Serviceauftrage')"> Serviceaufträge </h4>

        <h4 class="text-uppercase ml-6" @click="changeRoute('Vertrag')"> Vertrag </h4>

        <h4 class="text-uppercase ml-6" @click="changeRoute('Postfach')"> Postfach </h4>

        <h4 class="text-uppercase ml-6" @click="changeRoute('PersonlicheDaten')"> Persönliche Daten </h4>
        <h4 class="text-uppercase ml-6" @click="changeRoute('password')">  Passwort </h4>
      </v-app-bar>
    </v-container>

    <v-main  >
      <v-container fluid class="pt-0 mt-0">
        <Nuxt />
      </v-container>
    </v-main>
    <v-section class="">
      <v-container>
        <v-row class="flex justify-space-around">
          <v-col cols="12" lg="3" md="12" sm="12">
            <h6 class="text-left mb-2">In Partnerschaft mit:</h6>
            <v-img
              :src="require('../assets/DVAG_Logo-Beratung_durch_Gold.png')"
              width="60%"
            ></v-img>
          </v-col>
          <v-col cols="12" lg="3" md="12" sm="12">
            <v-img
              :src="
                require('../assets/logo_footer_geiger_aktiengesellschaft.png')
              "
              width="80%"
              class="mt-5"
            ></v-img>
          </v-col>
          <v-col cols="12" lg="3" md="12" sm="12">
            <h3>Hotline: 034206 180 111</h3>
            <h6>
              E-Mail: service@geiger-goldsparplan.de <br />
              Web: www.geiger-goldsparplan.de
            </h6>
          </v-col>
        </v-row>
        <hr  class="mt-5"/>

      </v-container>
    </v-section>
    <div class="text-center">
      <span
        >Copyright &copy; {{ new Date().getFullYear() }} All Rights
        Reserved</span
      >
    </div>
  </v-app>
</template>

<script>
import lazyLoad from "vue-lazyload";
export default {
  components: { lazyLoad },
  name: "DefaultLayout",
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      src: "",
      right: true,
      rightDrawer: false,
    };
  },
  methods: {
    changeRoute(route){
      console.log(this.$route.path)
      this.$router.push(route)
    }
  },
  computed: {},
};
</script>
<style scoped >
.background {
  background-color: black;
}
.text {
  color: #ffda6d;
}

.borderRadius {
  border-radius: 0px !important;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: #EEEEEE
;
}
.border{
  border-top: 10px solid #ffda6d !important;
  border-bottom: 1px solid #000000 !important;

}
.headerImage{
  position: relative;
  left: 100px;
}


</style>
