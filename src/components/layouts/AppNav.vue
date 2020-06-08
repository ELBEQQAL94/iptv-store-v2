<template>
<header>
  <v-container>
    <v-toolbar dark flat>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-toolbar-title>
        <Tv />
      </v-toolbar-title>
      <v-btn ref="button" @click="$vuetify.goTo('#accueil')" text>
        <v-toolbar-title>IPTV SMART</v-toolbar-title>
      </v-btn>

      <v-spacer></v-spacer>

      <v-btn ref="button" @click="$vuetify.goTo('#accueil')" text>
        <span class="mr-2">accueil</span>
      </v-btn>
      <v-btn ref="button" @click="$vuetify.goTo('#applications')" text>
        <span class="mr-2">applications</span>
      </v-btn>
       <v-btn ref="button" @click="$vuetify.goTo('#prices')" text>
        <span class="mr-2">prix</span>
      </v-btn>
      <v-btn ref="button" @click="$vuetify.goTo('#nos-offres')" text>
        <span class="mr-2">nos offres</span>
      </v-btn>
    </v-toolbar>
  </v-container>
</header>
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
