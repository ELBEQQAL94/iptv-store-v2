<template>
  <v-app>
    <v-app-bar
      app
      color="#000000"
      dark
    >
      <div class="d-flex align-center">
        <Tv />
        <!-- <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
          hidden-sm-and-down
        /> -->
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

    <v-content>
      <div id="accueil" style="width:100vw; height:100vh; background-color:blue;">Accueil</div>
      <div id="nos-offres" style="width:100vw; height:100vh; background-color:red;">Nos Offres</div>
    </v-content>
  </v-app>
</template>

<script>
import Tv from '@/components/icons/Tv.vue';

export default {
  name: 'App',

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
