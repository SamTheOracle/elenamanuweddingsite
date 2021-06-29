<template>
  <v-container>
    <div class="component-title text-center">Informazioni</div>
    <div class="component-subtitle text-center mt-6">
      Sarà necessario avere con sè il proprio GreenPass
    </div>
    <v-list>
      <v-list-item three-line v-for="(info, index) in infos" :key="index">
        <v-list-item-avatar>
            <v-img :src="require('@/assets/'+info.icon)"></v-img>
          </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title class="list-item-title">{{ info.title }}</v-list-item-title>
          <v-list-item-subtitle class="list-item-subtitle">{{ info.subtitle }}</v-list-item-subtitle>
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
      {
        title: "Vaccinazione",
        subtitle: "Se con una sola dose, occorre siano passati 14 giorni",
        icon: "vaccine.svg",
      },
      {
        title: "Guarigione dal virus",
        subtitle:
          "Portare un certificato di avvenuta guarigione ASUR risalente al massimo ai 6 mesi precedenti",
        icon: "certificate.svg",
      },
      {
        title: "Un tampone di qualsiasi tipo ",
        subtitle: "Molecolare, rapido, salivare) entro le 48 ore precedenti. ",
        icon: "swab.svg",
      },
    ],
  }),
};
</script>

<style>
</style>