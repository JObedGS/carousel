<template>
  <v-app>

  <v-carousel>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    ></v-carousel-item>
  </v-carousel>


  </v-app>
</template>

<script>


export default {
  name: 'App',

   data () {
      return {
        items: [
          {
            src: 'https://dsaenzh.com/webdesign2020/AbrahamAguilar/1.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
          },
        ],
      }
    },
};
</script>

<style scoped>

</style>