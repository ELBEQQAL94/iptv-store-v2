<template>
  <section class="heroBlock">
    <v-carousel show-arrows-on-hover cycle>
      <v-carousel-item
        v-for="(item, i) in items"
        :key="i"
        :src="item.src"
        reverse-transition="fade-transition"
        transition="fade-transition"
      ></v-carousel-item>
      </v-carousel>
  </section>
</template>

<script>

export default {
  name: 'Carousel',
  data() {
    return {
      items: [
        {
          src: 'https://images.unsplash.com/photo-1560169897-fc0cdbdfa4d5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=80',
        },
        {
          src: 'https://images.unsplash.com/photo-1461151304267-38535e780c79?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=80',
        },
        {
          src: 'https://images.unsplash.com/photo-1556889487-b6f8d3fc728b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80',
        },
        {
          src: 'https://images.unsplash.com/photo-1547130542-00f463cf8c0c?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80',
        },
        {
          src: 'https://images.unsplash.com/photo-1521967906867-14ec9d64bee8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=80',
        },
      ],
    };
  },
};
</script>
