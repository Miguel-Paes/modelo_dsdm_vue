<script setup></script>

<template>
  <v-app-bar class="d-flex flex-column text-center" color="brown-darken-1">
    <v-app-bar-title>Cronograma - 📙 Projeto da Biblioteca de Arcadia 📙</v-app-bar-title>
  </v-app-bar>

  <v-card class="bg-brown-lighten-1 mt-3 mx-16 d-flex" variant="tonal">
    <v-row>
      <v-col class="text-center d-flex flex-column justify-center align-center" cols="4">
        <v-card-title class="w-33">8 Meses</v-card-title>
        <v-card-text class="w-33">Duração Total</v-card-text>
      </v-col>

      <v-col class="text-center d-flex flex-column justify-center align-center" cols="4">
        <v-card-title class="w-33">5 Etapas</v-card-title>
        <v-card-text class="w-33">Ciclo de Vida</v-card-text>
      </v-col>

      <v-col class="text-center d-flex flex-column justify-center align-center" cols="4">
        <v-card-title class="w-33">3 Entregas</v-card-title>
        <v-card-text class="w-33">Módulos do Projeto</v-card-text>
      </v-col>
    </v-row>
  </v-card>

  <v-divider class="pa-1 my-3" color="white" />

  <v-card class="rounded-xl pa-3 mx-16" color="white">
    <v-card class="pa-3 rounded-xl" color="grey-lighten-5">
      <div class="rounded-xl">
        <v-card-title class="bg-brown-darken-4 rounded-t-xl">Etapa 1: Análise de Viabilidade</v-card-title>
        <v-card-text class="d-flex pt-3 bg-brown-lighten-5 border-colored">Define se é possível realizar o projeto com o prazo e orçamento oferecido</v-card-text>
      </div>
    </v-card>
  </v-card>
</template>

<style scoped>
  .border-colored {
    border-left: solid .5rem #3E2723;
  }
</style>
