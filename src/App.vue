<template>
  <v-app>
    <v-app-bar app color="white" light dense inverted-scroll>
      <v-spacer />
      <v-app-title class="main-title">Elena e Emanuele</v-app-title>
      <v-spacer />
    </v-app-bar>

    <v-main>
      <welcome />
      <date />
      <v-divider class="mx-4 ma-4" />
      <party />
      <v-divider class="mx-4 ma-4" />
      <useful-info />
    </v-main>
  </v-app>
</template>

<script>
import Date from "./components/Date.vue";
import Party from "./components/Party.vue";
import UsefulInfo from "./components/UsefulInfo.vue";
import Welcome from "./components/Welcome.vue";

export default {
  name: "App",

  components: {
    Welcome,
    Date,
    Party,
    UsefulInfo,
  },
  data: () => ({
    //
  }),
};
</script>
<style>
.main-title {
  font-family: "Satisfy", cursive;
  font-size: 34px;
}
.component-subtitle {
  font-family: "Montserrat", sans-serif;
  font-size: 20px;
  font-weight: 300;
  white-space: pre-line;
}
.component-title {
  font-family: "Dosis", sans-serif;
  line-height: 40px;
  font-size: 38px;
  font-weight: 400;
  white-space: pre-line;
}
.button-subtitle {
  font-family: "Montserrat", sans-serif;
  font-size: 15px;
  font-weight: 300;
  white-space: pre-line;
}
</style>