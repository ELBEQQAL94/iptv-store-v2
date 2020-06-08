<template>
  <div id="prices" class="block main-section">
    <v-container>
      <h2 class="text-center mt-12 mb-4">Vous Cherchez Un Abonnement IPTV moins chère?</h2>
      <v-row>
        <v-col v-for="item in items" :key="item.id" cols="12" md="4">
          <v-card class="mx-auto" max-width="400" height="500" hover>
            <v-list-item two-line>
              <v-list-item-content>
                <v-list-item-title class="headline">Dhs {{item.price}}</v-list-item-title>
                <v-list-item-subtitle>{{item.duree}}</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-icon>
                <Check />
              </v-list-item-icon>
              <v-list-item-subtitle>+19000 Dernières VOD a jour</v-list-item-subtitle>
            </v-list-item>
            <v-list-item>
              <v-list-item-icon>
                <Check />
              </v-list-item-icon>
              <v-list-item-subtitle>Compatible avec tous les appareils</v-list-item-subtitle>
            </v-list-item>
            <v-list-item>
              <v-list-item-icon v-if="item.isAllowed">
                <NotAllowed />
              </v-list-item-icon>
              <v-list-item-icon v-else>
                <Check />
              </v-list-item-icon>
              <v-list-item-subtitle>Assistance technique</v-list-item-subtitle>
            </v-list-item>
            <v-divider></v-divider>
            <v-card-actions>
              <v-btn
                :href="whatssapUrl"
                target="_blank"
                block
                ref="button"
                color="#ffffff"
                class="mt-8"
                rounded
                @click="$vuetify.goTo('#nos-offres')"
                text
                large
              >
                <span>Commander Par Whatssap</span>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import Check from '@/components/icons/Check.vue';
import NotAllowed from '@/components/icons/NotAllowed.vue';

export default {
  name: 'Prices',
  components: {
    Check,
    NotAllowed,
  },
  data() {
    return {
      whatssapUrl: 'https://api.whatsapp.com/send?phone=2120648488032&text=je%20suis%20int%C3%A9ress%C3%A9%20Par%20Votre%20offre%20Iptv&source=&data=&app_absent=',
      items: [
        {
          id: 1,
          price: '0.00',
          duree: '24 Hours',
          isAllowed: true,
        },
        {
          id: 1,
          price: '299.99',
          duree: '12 Mois',
          isAllowed: false,
        },
        {
          id: 1,
          price: '189.99',
          duree: '6 Mois',
          isAllowed: false,
        },
      ],
    };
  },
};
</script>
