<template>
  <v-container fluid>
    <div class="main-title text-center mb-4">Elena e Emanuele</div>
    <v-img
      v-if="$vuetify.breakpoint.smAndDown"
      max-height="800px"
      max-width="800px"
      class="mx-auto"
      transition="fade-transition"
      src="@/assets/front-pic.jpg"
    >
    </v-img>
    <v-img
      v-else
      max-height="1300px"
      class="mx-auto"
      transition="fade-transition"
      src="@/assets/front-pic-desktop.jpg"
    >
    </v-img>
      </v-container>
</template>

<script>
export default {
  name: "Welcome",
};
</script>

<style>
</style>

