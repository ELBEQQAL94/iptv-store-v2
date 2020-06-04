<template>
  <v-app-bar
      app
      color="#000000"
      dark
    >
      <div class="d-flex align-center">
        <Tv />
        <h1 class="hidden-sm-and-down">IPTV SMART</h1>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        ref="button"
        @click="$vuetify.goTo('#accueil')"
        text
      >
        <span class="mr-2">Accueil</span>
      </v-btn>
      <v-btn
        ref="button"
        @click="$vuetify.goTo('#nos-offres')"
        text
      >
        <span class="mr-2">Nos Offres</span>
      </v-btn>
    </v-app-bar>
</template>

<script>
import Tv from '../icons/Tv.vue';

export default {
  name: 'AppNav',
  components: {
    Tv,
  },
};
</script>

<style scoped>
h1 {
  color: #e50914;
}
</style>
