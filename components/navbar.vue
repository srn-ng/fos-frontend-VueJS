<template>
  <v-app-bar app color="white" flat hide-on-scroll prominent class="navbar">
      <v-toolbar-title>
        <!-- <v-img src="/images/logo-color 1.png" > </v-img> -->
 
      </v-toolbar-title>
      <div class="test ml-auto">
        <v-btn text to="/" class="navbar-button">Accueil</v-btn>
        <v-btn text to="/about" class="navbar-button">A propos</v-btn>
        <v-btn text to="/programme" class="navbar-button">Le Programme</v-btn>
        <v-btn text to="/partenaire" class="navbar-button">Partenaires</v-btn>
        <v-btn text to="/faq" class="navbar-button">FAQ</v-btn>
        <v-btn text to="/contact" class="navbar-button">Contact</v-btn>
        <v-btn elevation="0" class=" navbar-button program">Rejoindre le programme</v-btn>
        <v-icon></v-icon>
      </div>
    </v-app-bar>
</template>

<script>
export default {

}
</script>

<style >
.program {
  border: solid;
  border-color: #046380;
  background-color: white !important;
  color: #046380 !important;
  border-width: 1px;
  margin:-20px;
}
.navbar-button:hover{
  background-color: transparent !important;
}

.navbar-button::before{
  background-color: transparent !important;
}
.navbar-button:focus{
    border:solid !important;
    border-bottom: #046380 !important;
}
.program:hover{
  background-color: #046380 !important;
  color: white !important;
}
.navbar{
  align-items: right !important;
}
</style>