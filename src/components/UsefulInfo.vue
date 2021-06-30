<template>
  <v-container>
    <div class="component-title text-center">Informazioni</div>
    <div class="component-subtitle text-center mt-6">
      Sarà necessario avere con sè il GreenPass
    </div>
    <div v-if="$vuetify.breakpoint.smAndDown">
      <v-list>
        <v-list-item three-line v-for="(info, index) in infos" :key="index">
          <v-list-item-avatar>
            <v-img :src="require('@/assets/' + info.icon)"></v-img>
          </v-list-item-avatar>
          <v-list-item-content>
            <v-list-item-title class="list-item-title">{{
              info.title
            }}</v-list-item-title>
            <v-list-item-subtitle class="list-item-subtitle">{{
              info.subtitle
            }}</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </div>
    <div v-else>
      <v-row dense class="mt-6" align="center" align-content="center">
        <v-col v-for="(info, index) in infos" :key="index">
          <v-card
            elevation="2"
            shaped
            class="ma-2"
            height="200px"
          >
            <v-card-title>
              <v-avatar>
                <v-img :src="require('@/assets/' + info.icon)"></v-img>
              </v-avatar>
              <span class="list-item-title ml-5" v-text="info.title"></span>
            </v-card-title>
            <v-card-text class="list-item-subtitle" v-text="info.subtitle"></v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </div>
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
        title: "Tampone",
        subtitle: "Molecolare, rapido, salivare entro le 48 ore precedenti. ",
        icon: "swab.svg",
      },
    ],
  }),
};
</script>

<style>
</style>