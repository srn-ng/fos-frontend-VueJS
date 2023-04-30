<template>
  <v-app>
    <navbar></navbar>
    <v-main>
      <nuxt />
    </v-main>
  </v-app>
</template> 
<script>
import navbar from '../components/navbar.vue'
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
  components:{
    navbar,
  }
}
</script>


