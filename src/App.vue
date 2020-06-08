<template>
  <v-app>
    <app-nav />
    <v-content>
      <Carousel />
      <a
        class="float"
        title="whatssap"
        :href="whatssapUrl"
        target="_blank"
      >
        <Whatssap />
      </a>
      <Parallax />
      <Prices />
    </v-content>
  </v-app>
</template>

<script>
import AppNav from '@/components/layouts/AppNav.vue';
import Carousel from '@/components/main/Carousel.vue';
import Parallax from '@/components/main/Parallax.vue';
import Prices from '@/components/main/Prices.vue';
import Whatssap from '@/components/icons/Whatssap.vue';

export default {
  name: 'App',
  components: {
    AppNav,
    Carousel,
    Parallax,
    Prices,
    Whatssap,
  },
  data() {
    return {
      whatssapUrl: 'https://api.whatsapp.com/send?phone=2120648488032&text=je%20suis%20int%C3%A9ress%C3%A9%20Par%20Votre%20offre%20Iptv&source=&data=&app_absent=',
    };
  },
};
</script>

<style scoped>
h1 {
  color: #e50914;
}
</style>
