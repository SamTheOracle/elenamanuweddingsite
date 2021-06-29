<template>
  <v-app>
    <v-app-bar app color="white" light dense inverted-scroll>
      <v-spacer />
      <v-toolbar-title class="toolbar-title"
        >Elena e Emanuele</v-toolbar-title
      >
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
  font-family: "Dosis", sans-serif;
  font-size: 34px;
  font-weight: 200;
}
.toolbar-title {
  font-family: "Dosis", sans-serif;
  font-size: 30px;
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
.list-item-title {
  font-family: "Dosis", sans-serif;
  font-size: 18px;
  font-weight: 600;
  white-space: pre-line;
}
.list-item-subtitle {
  font-family: "Montserrat", sans-serif;
  font-size: 15px;
  font-weight: 300;
  -webkit-line-clamp: 5 !important;
}

@media only screen and (min-width: 601px) {
  .component-subtitle {
    font-size: 30px;
  }
  .component-title {
    font-size: 45px;
  }
  .button-subtitle {
    font-size: 20px;
  }
}
</style>