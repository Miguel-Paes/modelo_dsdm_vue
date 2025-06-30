<script setup>
  import { ref } from 'vue'

  import FifthStep from '@/components/FifthStep.vue'
  import FirstStep from '@/components/FirstStep.vue'
  import FourthStep from '@/components/FourthStep.vue'
  import SecondStep from '@/components/SecondStep.vue'
  import ThirdStep from '@/components/ThirdStep.vue'

  const tab = ref('step_one')
</script>

<template>
  <v-app-bar class="d-flex flex-column text-center" color="teal-darken-1">
    <v-app-bar-title>Cronograma - 🚑 Projeto da DrogaCara 🚑</v-app-bar-title>
  </v-app-bar>

  <v-card class="bg-teal-lighten-1 mt-3 mx-16 d-flex" variant="tonal">
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
      <v-tabs
        v-model="tab"
        align-tabs="center"
        bg-color="teal-darken-4"
        class="rounded-pill"
      >
        <v-tab value="step_one">Análise de Viabilidade</v-tab>
        <v-tab value="step_two">Análise de Negócio</v-tab>
        <v-tab value="step_three">Iteração do Modelo Funcional</v-tab>
        <v-tab value="step_four">Elaboração e Construção</v-tab>
        <v-tab value="step_five">Desenvolvimento e Implementação</v-tab>
      </v-tabs>

      <v-card-text>
        <v-tabs-window v-model="tab">
          <v-tabs-window-item value="step_one">
            <FirstStep />
          </v-tabs-window-item>

          <v-tabs-window-item value="step_two">
            <SecondStep />
          </v-tabs-window-item>

          <v-tabs-window-item value="step_three">
            <ThirdStep />
          </v-tabs-window-item>

          <v-tabs-window-item value="step_four">
            <FourthStep />
          </v-tabs-window-item>

          <v-tabs-window-item value="step_five">
            <FifthStep />
          </v-tabs-window-item>
        </v-tabs-window>
      </v-card-text></v-card>
  </v-card>
</template>

<style>
  .border-colored {
    border-left: solid .5rem #004D40;
  }
</style>
