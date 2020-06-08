<template>
  <section id="accueil" class="main-section">
    <v-parallax dark style="height:100%" src="https://cdn.vuetifyjs.com/images/parallax/material2.jpg">
      <v-row align="center" justify="center">
        <v-col class="text__center" md="6" xs="12">
          <h1 class="black--text font-weight-bold display-1 mb-4">
            Le Meilleur Service Iptv Au Maroc
          </h1>
          <div class="description mb-4 mt-4">
            <p class="font-italic font-weight-light">
              Avec EcomTec Vos émissions et chaînes
              favoris sur n’importe quel appareil, quel que
              soit votre emplacement. Plus de 7000 chaînes de
              télévision en direct et VOD SUR
              VOTRE TV, ORDINATEUR, TABLETTE OU SMARTPHONE.
            </p>
          </div>
          <v-btn
            block
            ref="button"
            color="#ffffff"
            class="mt-8"
            rounded
            @click="$vuetify.goTo('#nos-offres')"
            text
            large
          >
            <span>Nos Offres</span>
          </v-btn>
          <Applications />
        </v-col>
      </v-row>
    </v-parallax>
  </section>
</template>

<script>
import Applications from '@/components/main/Applications.vue';

export default {
  name: 'Parallax',
  components: {
    Applications,
  },
};
</script>
