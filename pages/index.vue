<template>
  <div class="py-9 px-10 md:px-[90px] pb-[406px] max-w-[1180px]">
    <div class="flex">
      <div class="">
        <h3 class="text-base text-gray-700 font-bold text-left mb-10">LOGIN</h3>

        <div>
          <div class="flex items-start space-x-2">
            <h4 class="black--text mt-2 caption">Nutzername</h4>
            <v-text-field outlined dense></v-text-field>
            <!-- <input type="text" class="border-2 border-gray-700" placeholder="test"> -->
          </div>

          <div class="flex items-start space-x-3">
            <h4 class="black--text mt-2 mr-4 caption">Passwort</h4>
            <v-text-field class="max-w-xl" outlined dense></v-text-field>
          </div>

          <div>
            <v-card-actions>
              <v-btn color="#ffda6d" class="text-capitalize px-6 borderRadius"
                >anmelden</v-btn
              >
            </v-card-actions>
          </div>
        </div>
      </div>
      <div></div>
    </div>
  </div>
</template>

<script>
import lazyLoad from "vue-lazyload";
export default {
  components: { lazyLoad },
  name: "IndexPage",
};
</script>
<style scoped>
.borderRadius {
  border-radius: 0px !important;
  margin-left: 5rem;
}

.v-text-field--outlined {
  border-radius: 0px;
  max-height: 50px !important;
}

.textfield {
  background-color: red;
  height: 20px;
}

.v-input.v-input--dense.theme--light.v-text-field.v-text-field--is-booted
  .v-text-field--enclosed.v-text-field--outlined {
  background: red !important;
  max-height: 20px !important;
}

.v-text-field--filled.v-input--dense.v-text-field--single-line
  > .v-input__control
  > .v-input__slot,
.v-text-field--filled.v-input--dense.v-text-field--outlined
  > .v-input__control
  > .v-input__slot,
.v-text-field--filled.v-input--dense.v-text-field--outlined.v-text-field--filled
  > .v-input__control
  > .v-input__slot,
.v-text-field--full-width.v-input--dense.v-text-field--single-line
  > .v-input__control
  > .v-input__slot,
.v-text-field--full-width.v-input--dense.v-text-field--outlined
  > .v-input__control
  > .v-input__slot,
.v-text-field--full-width.v-input--dense.v-text-field--outlined.v-text-field--filled
  > .v-input__control
  > .v-input__slot,
.v-text-field--outlined.v-input--dense.v-text-field--single-line
  > .v-input__control
  > .v-input__slot,
.v-text-field--outlined.v-input--dense.v-text-field--outlined
  > .v-input__control
  > .v-input__slot,
.v-text-field--outlined.v-input--dense.v-text-field--outlined.v-text-field--filled
  > .v-input__control
  > .v-input__slot {
  min-height: 15px !important;
}
</style>
