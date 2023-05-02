<template>
  <v-app-bar app color="white" flat hide-on-scroll prominent>
      <v-toolbar-title>
        <v-img src="/images/logo-color 1.png" class="img"> </v-img>
 
      </v-toolbar-title>
      <div class="ml-auto button-group">
        <v-btn text to="/" class="navbar-button">Accueil</v-btn>
        <v-btn text to="/about" class="navbar-button">A propos</v-btn>
        <v-btn text to="/programme" class="navbar-button">Le Programme</v-btn>
        <v-btn text to="/partenaire" class="navbar-button">Partenaires</v-btn>
        <v-btn text to="/faq" class="navbar-button">FAQ</v-btn>
        <v-btn text to="/contact" class="navbar-button">Contact</v-btn>
        <v-btn elevation="0" class=" navbar-button program">Rejoindre le programme</v-btn>
        <v-icon class="icon"> mdi-web</v-icon>
      </div>
    </v-app-bar>
</template>

<script>
export default {

}
</script>

<style >

.button-group {
  display: flex;
  height: 100%;
  align-items: center;
  justify-content: flex-end;
}

.button-group > * {
  color:#2D2D2D !important;
  margin-left: 16px;
  margin-right: 16px;
  font-size: 9pt !important;

}

.navbar-button:hover{
  background-color: transparent !important;
}
.navbar-button::before{
  background-color: transparent !important;
}
.program {
  border: solid;
  border-color: #046380;
  background-color: white !important;
  color: #046380 !important;
  border-width: 1px;
  border-radius: 10px !important;
}
.program:hover{
  background-color: #046380 !important;
  color: white !important;
  
}

.icon.mdi:before {
  color: #2D2D2D !important;
  font-size: 25px !important;
}

.img{
  margin-bottom: -20px;
}
</style>