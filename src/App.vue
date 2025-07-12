<template>
  <v-app>
    <v-main>
      <MelhoriasIgreja/>
    </v-main>
  </v-app>
</template>

<script>
import MelhoriasIgreja from './components/MelhoriasIgreja.vue'

export default {
  name: 'App',

  components: {
    MelhoriasIgreja,
  },

  data: () => ({
    //
  }),
}
</script>
