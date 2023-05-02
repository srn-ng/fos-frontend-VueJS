<template>
  <v-app>
    <navbar></navbar>
    <v-main>
      <index id="index" />
      <overview id="about" />
      <contenu id="contenu" />
      <calendar id="calendar" />
      <partners id="partners" />
    </v-main>
  </v-app>
</template> 
<script>
import navbar from '../components/navbar.vue'
import index from '../pages/index.vue'
import overview from '../pages/overview.vue'
import calendar from '../pages/calendar.vue'
import contenu from '../pages/content.vue'
import partners from '../pages/partners.vue'


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
    navbar,
    index,
    overview,
    calendar,
    contenu,
    partners,
  },
}
</script>
<style >
</style>


