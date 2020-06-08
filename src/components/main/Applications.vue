<template>
  <v-row id="applications">
    <v-col v-for="item in items" :key="item.id" class="d-flex child-flex" cols="6" sm="6">
      <v-card flat tile class="d-flex">
        <v-img :src="item.src" aspect-ratio="1" class="grey lighten-2">
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'Applications',
  data() {
    return {
      items: [
        {
          id: 1,
          src: 'https://cdn6.aptoide.com/imgs/7/6/c/76c56660d42b4a616b294bea8388bb7c_icon.png?w=256',
        },
        {
          id: 2,
          src: 'https://www.smart-iptv.info/wp-content/uploads/2018/11/smartiptvlogo.png',
        },
      ],
    };
  },
};
</script>
