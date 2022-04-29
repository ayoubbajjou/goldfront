<template>
  <v-container class="pa-0">
    <v-card>
      <v-card-text>

    <v-row>
      <v-col cols="12" lg="5" md="12" sm="12">
        <v-row>
          <v-col cols="12" lg="12" md="12" sm="12">
            <h3>MEINE UMSÄTZE
</h3>
          </v-col>
          <v-col cols="12" lg="4" sm="12" md="12">
<v-text-field outlined dense label="von
01.01.2022
" class="mt-7"></v-text-field>
          </v-col>
          <v-col cols="12" lg="4" sm="12" md="12">
<v-text-field outlined dense label="bis
27.04.2022
" class="mt-7"></v-text-field>

          </v-col>
          <v-col cols="12" lg="3" sm="12" md="12">
 <v-card-actions>
<v-btn color="#ffda6d" class="text-capitalize px-6 borderRadius mt-5 ">Download</v-btn>
</v-card-actions>
          </v-col>
          <v-col cols="12" lg="12" md="12" sm="12">
            <p>Keine Umsätze gefunden.

</p>
          </v-col>
        </v-row>

      </v-col>
    </v-row>

      </v-card-text>
    </v-card>
  </v-container>
</template>

<script>
  export default {
layout:'innerLayout'
  }
</script>
<style>
.v-text-field--outlined > .v-input__control > .v-input__slot {
    max-height: 20px !important;
    min-height: 30px !important;
    width: 200px !important;
    border-radius: 0px !important;

}

.v-input.v-input--dense.theme--light.v-text-field.v-text-field--is-booted .v-text-field--enclosed.v-text-field--outlined{
    background: red !important;
    max-height: 20px !important;

}
.borderRadius{
  border-radius: 0px !important;
}
</style>

<style lang="scss" scoped>

</style>
