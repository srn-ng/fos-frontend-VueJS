<template>
  <v-app>
    <navbar @change-drawer="handleEmit"></navbar>
    <v-main>
      <index id="index" />
      <overview id="about" />
      <contenu id="contenu" />
      <calendar id="calendar" />
      <partners id="partners" />
      <faq id="faq"/>
      <contact id="contact"/>
    </v-main>
    <v-navigation-drawer v-model="drawer">
      <v-list nav dense>
        <v-list-item-group active-class="deep-purple--text text--accent-4">
          <v-list-item>
            <v-list-item-title>Foo</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Bar</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Fizz</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Buzz</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
    <v-footer app absolute color="#D9D9D9" height="128px">
      <v-img src="/images/logo.png" class="imagess"></v-img>

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
  methods: {
    handleEmit() {
      console.log("emit received")
      this.drawer = ! this.drawer
    }
  }
}
</script>
<style >
.imagess {

  max-width: 10%;
}
</style>


