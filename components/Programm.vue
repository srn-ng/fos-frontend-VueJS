<template>
  <div class="d-flex justify-center mt-5 pt-5 pb-4">
    <v-row justify="center">
      <v-col cols="10" md="6">
        <div class="d-flex justify-center">
          <div>
            <h4 style="font-size: 2rem; color: #046380">Le programme</h4>
            <v-divider class="my-4" color="#046380" width="25%"></v-divider>
          </div>
        </div>
        <v-card>
          <v-card-text>
            <p class="description">
              Ce programme est à destination des jeunes diplômés en ingénierie
              des universités et écoles algériennes. D’un côté, les jeunes font
              état de difficultés à s’insérer sur le marché du travail à l’issue
              de leur diplomation, localement comme à l’international. De
              l’autre, les entreprises souffrent d’une inadéquation entre la
              formation initiale des jeunes diplômés et leurs besoins.

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
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </div>
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
.description {
  color: #6e6b80;
}
</style>