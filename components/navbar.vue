<template>
  <div>
    <v-app-bar app color="white" flat hide-on-scroll class="NavBar">
      <v-toolbar-title>
        <v-img class="logoNavBar" src="/images/logo.png"> </v-img>
      </v-toolbar-title>

      <div class="ml-auto button-group hidden-sm-and-down">
        <v-btn text to="#index" class="navbar-button">Accueil</v-btn>
        <v-btn text to="#about" class="navbar-button">A propos</v-btn>
        <v-btn text to="#calendar" class="navbar-button">Le Programme</v-btn>
        <v-btn text to="#partners" class="navbar-button">Partenaires</v-btn>
        <v-btn text to="#faq" class="navbar-button">FAQ</v-btn>
        <v-btn text to="#contact" class="navbar-button">Contact</v-btn>
        <!-- <v-btn elevation="0" class=" navbar-button program">Rejoindre le programme</v-btn> -->
      </div>

      <v-menu offset-y v-model="menuOpen">
        <template v-slot:activator="{ on }">
          <v-btn icon v-on="on" class="d-sm-none" @click="toggleMenu">
            <v-icon>mdi-menu</v-icon>
          </v-btn>
        </template>
        <v-list>
          <v-list-item
            v-for="(button, index) in mobileButtons"
            :key="index"
            @click="navigate(button.to)"
          >
            <v-list-item-title>{{ button.label }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      menuOpen: false,
      mobileButtons: [
        { label: 'Accueil', to: '#index' },
        { label: 'A propos', to: '#about' },
        { label: 'Le Programme', to: '#calendar' },
        { label: 'Partenaires', to: '#partners' },
        { label: 'FAQ', to: '#faq' },
        { label: 'Contact', to: '#contact' },
      ],
    }
  },
  methods: {
    test() {
      this.$emit('change-drawer')
    },
    toggleMenu() {
      this.menuOpen = !this.menuOpen
    },

    navigate(to) {
      this.$router.push(to)
    },
  },
}
</script>

<style >
.NavBar {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 999;
  padding: 0 1% 0 2%;
}
.button-group {
  display: flex;
  /* height: 100%; */
  align-items: center;
  justify-content: flex-end;
}

.button-group > * {
  color: #000000;
  margin-right: 2%;
  font-size: 60% !important;
  font-weight: 600;
  font-family: Montserrat;
}

.navbar-button:hover {
  background-color: transparent !important;
  color: #19a5cf;
  font-weight: 800;
}
.navbar-button a {
  color: #000; /* Couleur du texte des liens */
  text-decoration: none; /* Supprime la soulignement des liens */
  transition: color 0.3s; /* Ajoute une transition de couleur de 0.3 seconde */
}

.navbar-button::before {
  background-color: transparent !important;
}

.program {
  border: solid;
  border-color: #046380;
  background-color: white !important;
  color: #046380 !important;
  border-width: 1px;
  border-radius: 10px !important;
  padding: 1%;
}

.program:hover {
  background-color: #046380 !important;
  color: white !important;
}

.icon.mdi:before {
  color: #2d2d2d !important;
  font-size: 25px !important;
}

.logoNavBar {
  height: 30%;
  width: 30%;
}
</style>