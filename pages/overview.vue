<template>
  <v-card style="margin-top: -20px" class="pb-5" fluid elevation="0">
    <v-img src="/images/Background-Polygon-2.png">
      <div class="divvv">
        <div style=" margin-top: 5%;">
          <h4 style="font-size: 2rem; color: #046380" class="program-title">Le programme</h4>
          <v-divider class="my-4" color="#046380" width="5%"></v-divider>
        </div>

        <div class="description-div">
          <p class="description">
            Ce programme est à destination des jeunes diplômés en ingénierie des
            universités et écoles algériennes. D’un côté, les jeunes font état
            de difficultés à s’insérer sur le marché du travail à l’issue de
            leur diplomation, localement comme à l’international. De l’autre,
            les entreprises souffrent d’une inadéquation entre la formation
            initiale des jeunes diplômés et leurs besoins.

            <br />
            <br />
            Face à ce constat, ce programme d’executive education offre à des
            jeunes diplômés, préalablement sélectionnés sur la base de leur
            motivation et de l’excellence de leur profil académique, une
            formation accélérée en trois mois.

            <br />
            <br />
            Cette formation est dispensée par des enseignants et acteurs du
            secteur privé issus des meilleures universités, écoles et
            entreprises étrangères, et donc au fait des standards
            internationaux.

            <br />
          </p>
        </div>
      </div>
    </v-img>
  </v-card>
</template>
<script>
import { VImg } from 'vuetify/lib'

export default {
  name: 'IndexPage',
  components: {
    VImg,
  },
}
</script>
<style>
@media only screen and (min-width: 601px) {
  .program-title{
    margin-left: 35%;
  }
  .description-div {
    margin-top: 5%;
    margin-left :10% ;
    margin-right: 30%;
    text-align: justify;
  }
}

@media only screen and (max-width: 600px) {
  .divvv {
    text-align: center;
    align-items: center;
  }

  .description-div {
    margin-top: 5%;
    margin-left: 5%;
    margin-right: 5%;
    text-align: justify;
  
  }
}

#program-line {
  position: absolute;
  margin: auto;
  top: 50%;
  transform: translateY(50%);
}

#program-text {
  position: relative;
  font-family: 'Montserrat semibold', sans-serif;
  font-size: 2rem;
  color: #046380;
}

.description {
  color: #6E6B80
}
</style>