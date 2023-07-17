<template>
  <v-app>
    <navbar @change-drawer="handleEmit"></navbar>
    <v-main>
      <home id="home" />
      <overview id="about" />
      <contenu id="contenu" />
      <calendar id="calendar" />
      <faq id="faq" />
      <contact id="contact" />
      <partners id="partners" />
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
      <v-img src="/images/logo.png" class="logo"></v-img>
    </v-footer>
  </v-app>
</template> 
  <script>
import navbar from '../layouts/navbar.vue'
import home from '../components/Home.vue'
import overview from '../components/Programm.vue'
import calendar from '../components/Calendar.vue'

import contenu from '../components/ProgrammContent.vue'
import partners from '../components/Partners.vue'

import faq from '../components/faq.vue'
import contact from '../components/Contact.vue'

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
          to: '/index',
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
    home,
    overview,
    calendar,
    contenu,
    partners,
    faq,
    contact,
  },
  methods: {
    handleEmit() {
      console.log('emit received')
      this.drawer = !this.drawer
    },
  },
}
</script>
  <style >
* {
  font-family: 'Montserrat', sans-serif;
}
.logo {
  max-height: 75px;
  max-width: 75px;
}
</style>
  
  
  