<template>
  <v-sheet>
    <p class="text-center mt-2 mb-0" style="white-spaces: pre-line;font-size:12px">
      Made with
      <span>
        <v-icon color="red">mdi-heart</v-icon>
      </span>
      by
    </p>
    <div  class="text-center">
    <v-btn
      :x-small="$vuetify.breakpoint.xsOnly"
      depressed
      @click="onOracleClick()"
      color="#607D8B"
      dark
      >Giacomo</v-btn
    >
    </div>
  </v-sheet>
</template>

<script>
export default {
  name: "MadeBy",
  methods:{
      onOracleClick(){
          window.open("https://www.linkedin.com/in/giacomozanotti")
      }
  }
};
</script>

<style>
</style>