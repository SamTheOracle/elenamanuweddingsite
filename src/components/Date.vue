<template>
  <v-container>
    <div class="component-title text-center">
      Annunciano con gioia il loro matrimonio
    </div>
    <div class="component-subtitle text-center mt-6">18 Settembre 2021</div>
    <div class="component-subtitle text-center">Alle ore 11:00</div>

    <div class="component-subtitle text-center mt-12">Chiesa di San Pietro Apostolo</div>
    <div class="component-subtitle text-center">Via XX Settembre</div>
    <div class="component-subtitle text-center">San Giovanni in Marignano (RN)</div>
    <confirm/>
  </v-container>
</template>

<script>
import Confirm from './Confirm.vue';
export default {
  components: { Confirm },
  name: "Date",
};
</script>

<style>
</style>