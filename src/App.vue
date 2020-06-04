<template>
  <v-app>
    <app-nav />

    <v-content>
      <div id="accueil" style="width:100vw; height:100vh; background-color:blue;">Accueil</div>
      <div id="nos-offres" style="width:100vw; height:100vh; background-color:red;">Nos Offres</div>
    </v-content>
  </v-app>
</template>

<script>
import AppNav from '@/components/layouts/AppNav.vue';

export default {
  name: 'App',

  components: {
    AppNav,
  },
};
</script>
