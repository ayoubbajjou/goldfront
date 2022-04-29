<template>
  <div id="app" light>
    <div class="block max-w-none md:max-w-[1180px] md:mx-auto">
      <div
        class="w-full background box pa-0 border max-w-none md:max-w-[1180px] md:mx-auto border-b-[10px] border-r-0 border-l-0 border-t-0 border-primary"
      >
        <div
          class="flex-col-reverse md:flex-row flex justify-between items-center"
        >
          <div class="w-full text-start mt-6">
            <h2
              class="text-[28px] text-white font-bold"
            >
              MEIN GEIGER GOLDSPARPLAN
            </h2>
            <h2 class="text-primary text-lg">
              Eine glänzende Idee für Ihre Zukunft!
            </h2>
          </div>
          <div class="flex items-center">
            <img
              :src="require('../assets/Geiger-goldsparplan-goldbarren-50g.png')"
              class="w-52 -mr-[105px] mt-[54px]"
            />
            <img
              :src="require('../assets/Header.png')"
              class="hidden md:block w-[480px] bg-cover mr-[600px] -mt-[46px]"
            />
          </div>
        </div>

        <!-- <v-app-bar class="elevation-0 border">
        <h4 class="text-uppercase" @click="changeRoute('Ubersicht')"
        > Übersicht </h4>
        <h4 class="text-uppercase ml-6" @click="changeRoute('Umsatze')"> Umsatze </h4>

        <h4 class="text-uppercase ml-6" @click="changeRoute('Serviceauftrage')"> Serviceaufträge </h4>

        <h4 class="text-uppercase ml-6" @click="changeRoute('Vertrag')"> Vertrag </h4>

        <h4 class="text-uppercase ml-6" @click="changeRoute('Postfach')"> Postfach </h4>

        <h4 class="text-uppercase ml-6" @click="changeRoute('PersonlicheDaten')"> Persönliche Daten </h4>
        <h4 class="text-uppercase ml-6" @click="changeRoute('password')">  Passwort </h4>


      </v-app-bar> -->
      </div>

      <v-main class="w-full">
        <div class="max-w-[1180px] bg-white md:mx-auto">
          <Nuxt />
        </div>
      </v-main>

      <!-- Footer -->
      <div
        class="max-w-none md:max-w-[1180px md:mx-auto py-5 border-b border-r-0 border-t-0 border-l-0 border-gray-800"
      >
        <div
          class="flex flex-col space-y-3 justify-between mx-auto items-center md:grid grid-col-3 grid-flow-col gap-4 px-16"
        >
          <div>
            <h6 class="text-left mb-2">In Partnerschaft mit:</h6>
            <img
              :src="require('../assets/DVAG_Logo-Beratung_durch_Gold.png')"
              class="w-[250px]"
            />
          </div>
          <div>
            <img
              :src="
                require('../assets/logo_footer_geiger_aktiengesellschaft.png')
              "
              class="mt-5 w-[300px] h-[55px]"
            />
          </div>
          <div>
            <h3>Hotline: 034206 180 111</h3>
            <h6>
              E-Mail: service@geiger-goldsparplan.de <br />
              Web: www.geiger-goldsparplan.de
            </h6>
          </div>
          <div>
            <div style="border-bottom: 2px solid grey; width: 100%"></div>
          </div>
        </div>
      </div>
      <div class="text-center mt-3">
        <span class="caption black--text"
          >Impressum | Datenschutzerklärung | © 2021 Geiger Edelmetalle AG</span
        >
      </div>
    </div>
  </div>
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
    changeRoute(route) {
      console.log(this.$route.path);
      this.$router.push(route);
    },
  },
  computed: {},
};
</script>
<style scoped>
.background {
  background: radial-gradient(circle, #484848 0%, #282828 100%);
  padding: 0px 90px;
}
/* .text {
  color: #ffda6d;
} */

/* .borderRadius {
  border-radius: 0px !important;
} */
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #e8e8e8;
}
/* .border{
  border-bottom: 10px solid #ffda6d !important;
} */
/* .headerImage{
  position: relative;
  left: 100px;
  top:100px
}

.box {
  height: 230px;
  width: 80%;

  display: flex;
  flex-direction: column;
  justify-content: flex-end;

} */
</style>
