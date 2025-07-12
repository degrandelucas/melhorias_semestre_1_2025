<template>
  <v-app>
    <v-carousel show-arrows="hover" :height="$vuetify.display.height">
      <v-carousel-item
        v-for="(item, i) in carouselItems"
        :key="i"
        :src="item.src"
        cover
      >
        <div class="d-flex align-start justify-start fill-height">
          <h2 class="text-white text-h4 ma-4">{{ item.title }}</h2>
        </div>
      </v-carousel-item>
    </v-carousel>
  </v-app>
</template>

<script>
export default {
  name: "MelhoriasIgreja",
  data: () => ({
    carouselItems: [
      { src: require("../assets/assets/lousa_escola_biblica.jpeg"), title: "Lousa Escola Bíblica Dominical" },
      { src: require("../assets/assets/sala_juniores.jpeg"), title: "Sala Juniores (Casinha)" },
      { src: require("../assets/assets/sala_criancas.jpeg"), title: "Sala Crianças (Casinha)" },
      { src: require("../assets/assets/cozinha_casinha.jpeg"), title: "Cozinha (Casinha)" },
      { src: require("../assets/assets/dispensa_alimentacao.jpeg"), title: "Alimentação, Itens de Limpeza, Estrutura para Armazenamento" },
      { src: require("../assets/assets/forro_armacao_1.jpeg"), title: "Armação nova para o Templo" },
      { src: require("../assets/assets/forro_armacao_2.jpeg"), title: "Armação nova para o Templo" },
      { src: require("../assets/assets/forro_quase_finalizado.jpeg"), title: "Forro quase sendo Finalizado" },
      { src: require("../assets/assets/forro_finalizado.jpeg"), title: "Novo Forro Igreja" },
      { src: require("../assets/assets/forro_novas_lampadas.jpeg"), title: "Novas Lâmpadas, Melhor Iluminação" },
      { src: require("../assets/assets/ventiladores.jpeg"), title: "2 Novos Ventiladores" },
      { src: require("../assets/assets/caixa_som_altar.jpeg"), title: "Nova Caixa de Som Retorno Altar" },
      { src: require("../assets/assets/caixa_som_lateral.jpeg"), title: "Nova Caixa de Som (Lateral do Tempo) e Pintura Paredes do Altar" },
    ],
  }),
};
</script>