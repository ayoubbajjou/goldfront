<template>
  <v-container class="pa-0">
    <v-card>
      <v-card-text>


    <v-row>
      <v-col cols="12" lg="12" md="12" sm="12" offset-lg="1">
        <h3 class="text-left my-5">MEINE SERVICEAUFTRÄGE
</h3>
      </v-col>
       <v-col cols="12" lg="4" md="6" sm="6" offset-lg="1">
         <h4 class="text-left">Dokument</h4>
<v-data-table
    :headers="headers"
    :items="desserts"
    :items-per-page="5"
    hide-default-footer
    hide-default-header

    class="elevation-0 mt-6"
  ></v-data-table>
       </v-col>
       <v-col cols="12" lg="1" md="6" sm="6" class="pl-0">
<v-btn color="#ffda6d" class="text-capitalize px-6 py-5 pt-6 borderRadius mt-12 ml-0">download</v-btn>
<v-btn color="#ffda6d" class="text-capitalize px-6 py-5 pt-6 borderRadius mt-1  ml-0">download</v-btn>
<v-btn color="#ffda6d" class="text-capitalize px-6 py-5 pt-6 borderRadius mt-1  ml-0">download</v-btn>
<v-btn color="#ffda6d" class="text-capitalize px-6 py-5 pt-6 borderRadius mt-1  ml-0">download</v-btn>

</v-col>
    </v-row>
</v-card-text>
    </v-card>
  </v-container>
</template>

<script>
  export default {
    layout:'innerLayout',
    data () {
      return {
        headers: [
          {
            text: 'Dokument',
            align: 'start',
            sortable: false,
            value: 'name',
          },


        ],
        desserts: [

          {
            name: 'Auftrag Sparplan/Kauf',
            align: 'start',

          },
          {
            name: 'Änderungs- und Transaktionsauftrag	'


          },
          {
            name: 'Vollmacht',

          },
          {
            name: 'Auftrag Depotübertrag	'

          },

        ],
      }
    },
  }
</script>

<style>
.theme--light.v-data-table > .v-data-table__wrapper > table > tbody > tr:not(:last-child) > td:last-child, .theme--light.v-data-table > .v-data-table__wrapper > table > tbody > tr:not(:last-child) > th:last-child {
    border-bottom: thin solid rgba(0, 0, 0, 0.12);
    text-align: left;
}
</style>
<style  scoped>
.borderRadius{
  border-radius: 0px !important;
}
</style>
