<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title>My App</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text to="#index">Accueil</v-btn>
      <v-btn text to="#about">A propos</v-btn>
      <v-btn text to="/programme">Programme</v-btn>
      <v-btn text to="/partenaire">Partenaires</v-btn>
      <v-btn text to="/faq">FAQ</v-btn>
      <v-btn text to="/contact">Contact</v-btn>
    </v-app-bar>
    <v-main>
      <index id="index" class="index"/>
      <about id="about" class="about" />

    </v-main>

  </v-app>
</template>

<script>
import index from "../pages/index.vue"
import about from "../pages/about.vue"

export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Accueil',
          to: '/accueil',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
  components: {
    index,
    about
  }
}
</script>
