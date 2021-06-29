<template>
  <v-container>
    <div class="text-center ma-2">
      <v-btn color="#95875E" @click="onJoinClick()" dark :x-large="$vuetify.breakpoint.lgAndUp" :large="$vuetify.breakpoint.mdOnly" >Partecipa</v-btn>
    </div>

    <div class="button-subtitle text-center">(Entro il 20 Agosto)</div>
  </v-container>
</template>

<script>
export default {
  name: "Confirm",
  methods:{
    onJoinClick(){
      window.open('https://docs.google.com/forms/d/e/1FAIpQLSfAWmuFa-lt6aCoJUvk_jtoLmEgkz5MqqZkrCGbFGPQibdx6Q/viewform?usp=pp_url')
    }
  }
};
</script>
