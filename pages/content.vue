
<template>
  <div class="scroll-container">
    <v-card style="margin-top: -20px" fluid elevation="0">
      <v-row class="my-row">
        <v-col cols="12" class="my-col">
          <v-img src="/images/Group-1.png" class="triangle"></v-img>
          <h4 class="titre">Formation théorique</h4>
          <p class="description">
            4 modules sont au programme des 2 semaines d’enseignement :
          <ul>
            <li>Software engineering;</li>
            <li>Data engineering;</li>
            <li>Statistiques;</li>
            <li>Leadership.</li>
          </ul>
          </p>
        </v-col>
        <v-col cols="12" class="my-col">
          <v-img src="/images/Group-2.png" class="triangle"></v-img>
          <h4 class="titre">Stage pratique</h4>
          <p class="description">
            Des stages pratiques de 6 semaines sont proposés par les entreprises
            partenaires permettant de mettre en application les notions abordées.
          </p>
        </v-col>
        <v-col cols="12" class="my-col">
          <v-img src="/images/Group-3.png" class="triangle"></v-img>
          <h4 class="titre">Conférences</h4>
          <p class="description">
            Des conférences bi-hebdomadaires seront animées par des professionnels
            issus du monde de l’entreprise. L’objectif poursuivi est double :
            donner à voir comment toutes ces technologies s’appliquent dans des
            domaines variés (santé, agriculture, énergie, transport…) et permettre
            aux étudiants de se constituer un premier réseau de qualité.
          </p>
        </v-col>
        <v-col cols="12" class="my-col">
          <v-img src="/images/Group-3.png" class="triangle"></v-img>
          <h4 class="titre">Coaching</h4>
          <p class="description">
            Un coaching personnalisé est assuré pour chacun des participants tout
            au long des 8 semaines.
          </p>
        </v-col>
      </v-row>
    </v-card>
  </div>
</template>

<script>
export default {}
</script>

<style>
@media screen and (max-width: 600px) {
  .scroll-container {
    overflow-x: scroll;
    white-space: nowrap;
  }

  .my-col {
    display: inline-block;
    vertical-align: top;
    width: 100%;
  }
  .my-row {
    margin: 5% 35px;
  
  }
  .description {
  color: #6e6b80;
  text-align: justify;
}
}

@media screen and (min-width: 601px) {
  .my-row {
    margin: 5% 80px;
    /* add left and right margins */
  }
  .description {
  color: #6e6b80;
}
}


.my-col {
  flex-basis: 0;
  flex-grow: 1;
}

.triangle {
  max-width: 30% !important;
  max-height: 30% !important;
}

.titre {
  margin-top: 5%;
  margin-bottom: 5%;
  font-size: 15pt !important;
}


</style>
