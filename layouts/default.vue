<template>
  <v-app>
    <navbar></navbar>
    <v-main>
      <index id="index" />
      <overview id="about" />
      <contenu id="contenu" />
      <calendar id="calendar" />
      <partners id="partners" />
      <faq id="faq"/>
      <contact id="contact"/>

    </v-main>
    <v-footer app absolute color="#D9D9D9" height="128px"  >
      <v-img src="/images/logo-color 1.png" class="imagess"></v-img> 

    </v-footer>

  </v-app>
</template> 
<script>
import navbar from '../components/navbar.vue'
import index from '../pages/index.vue'
import overview from '../pages/overview.vue'
import calendar from '../pages/calendar.vue'
import contenu from '../pages/content.vue'
import partners from '../pages/partners.vue'

import faq from "../pages/faq.vue"
import contact from "../pages/contact.vue"


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
    faq,
    contact
  },
}
</script>
<style >
.imagess{
  width:142px !important;
  display:block !important;
  margin-top: 10px !important;
  height: 100% !important;
max-width: 15%; 
}
</style>


