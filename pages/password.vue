<template>
  <v-container class="pa-0">
    <v-card elevation="0" flat class="mt-0">
<v-card-text>
  <h3 class="text-left ml-12 mt-5">ÄNDERUNG PASSWORT
</h3>
   <v-row class="mt-10">
      <v-col cols="12" lg="6" md="12" sm="12" offset-lg="1">



        <v-row>
          <v-col cols="12" lg="3" md="12" sm="12">
            <h4 class="black--text caption text-left mt-2">
            Passwort alt	</h4>
            </v-col>
          <v-col cols="12" lg="7" md="12" sm="12">
            <v-text-field outlined dense></v-text-field>
          </v-col>

          <v-col cols="12" lg="3" md="12" sm="12">
           <h4 class="black--text mt-2 text-left caption  mr-4"> Passwort neu
             </h4>
           </v-col>

          <v-col cols="12" lg="7" md="12" sm="12">
            <div class="textfield" >
            <v-text-field outlined dense  ></v-text-field>
</div>

          </v-col>
          <v-col cols="12" lg="3" md="12" sm="12">
            <h4 class="black--text text-left caption mt-2">
            Passwortbestätigung		</h4>
            </v-col>
          <v-col cols="12" lg="7" md="12" sm="12">
            <v-text-field outlined dense></v-text-field>
            <v-card-actions>
<v-btn width="200" color="#ffda6d" class="text-capitalize px-6 ml-0 borderRadius mt-5 ">anmelden</v-btn>
</v-card-actions>
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

<style  scoped>
.v-text-field--outlined {
    border-radius: 0px;
    max-height: 20px !important;
}
</style>
