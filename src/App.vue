<template>
  <v-app>
    <nav-bar></nav-bar>
    <main-section></main-section>
    <item-section-1></item-section-1>
  </v-app>
</template>

<script>
import NavBar from './components/NavBar.vue';
import MainSection from './components/MainSection.vue';
import ItemSection1 from './components/ItemSection1.vue';

export default {
  components: {
    NavBar,
    MainSection,
    ItemSection1,
  },

};
</script>
