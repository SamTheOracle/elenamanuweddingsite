<template>
  <v-container>
    <div class="component-title text-center">Informazioni</div>
    <div class="component-subtitle text-center mt-6">
      Sarà necessario avere con sè il proprio GreenPass
    </div>
    <v-list>
      <v-list-item v-for="(info, index) in infos" :key="index">
        <v-list-item-content>
          <v-list-item-title v-text="info" />
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </v-container>
</template>

<script>
export default {
  name: "UsefulInfo",
  data: () => ({
    infos: [
      "Essere vaccinati (se con una sola dose, occorre siano passati almeno 14 giorni).",
      "Essere guariti dal virus (mostrando un certificato di avvenuta guarigione ASUR risalente al massimo ai 6 mesi precedenti)",
      "Un tampone di qualsiasi tipo (molecolare, rapido, salivare) entro le 48 ore precedenti. ",
    ],
  }),
};
</script>

<style>
</style>