<template>
  <v-container class="pa-0">
    <v-card>
      <v-card-text>


    <v-row>
      <v-col cols="12" lg="12" md="12" sm="12">
        <h3 class="text-left">MEINE SERVICEAUFTRÄGE
</h3>
      </v-col>
       <v-col cols="12" lg="10" md="6" sm="6">
<v-data-table
    :headers="headers"
    :items="desserts"
    :items-per-page="5"
    hide-default-footer

    class="elevation-0 "
  ></v-data-table>
       </v-col>
       <v-col cols="12" lg="1" md="6" sm="6" class="pl-0">
<v-btn color="#ffda6d" class="text-capitalize px-6 py-5 pt-6 borderRadius mt-12 ml-0">download</v-btn>
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
            align: 'center',
            sortable: false,
            value: 'name',
          },
          {
            text: 'Datum',
            align: 'center',
            sortable: false,
            value: 'name',
          },
          {
            text: 'Status',
            align: 'center',
            sortable: false,
            value: 'name',
          },


        ],
        desserts: [

          {
            name: 'Auftrag Sparplan/Kauf',
            Datum:'11.02.2021	',
            Status:'gelesen - 06.04.2022'
          },
          {
            name: 'Auftrag Sparplan/Kauf',
            Datum:'11.02.2021	',
            Status:'gelesen - 06.04.2022'
          },
          {
            name: 'Auftrag Sparplan/Kauf',
            Datum:'11.02.2021	',
            Status:'gelesen - 06.04.2022'
          },


        ],
      }
    },
  }
</script>

<style  scoped>
.borderRadius{
  border-radius: 0px !important;
}
</style>
