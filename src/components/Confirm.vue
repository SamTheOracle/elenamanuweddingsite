<template>
  <v-container>
    <div class="text-center ma-2">
      <v-btn color="success" dark :x-large="$vuetify.breakpoint.lgAndUp" :large="$vuetify.breakpoint.mdOnly" >Partecipa</v-btn>
    </div>

    <div class="button-subtitle text-center">(Entro il 20 Agosto)</div>
  </v-container>
</template>

<script>
export default {
  name: "Confirm",
};
</script>
