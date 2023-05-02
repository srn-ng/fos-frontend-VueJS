<template>
  <v-card class="pb-5" fluid elevation="0">
    <v-img src="/images/Background-Polygon-1.png">

      <v-row>
        <v-col cols="4" style="margin-top: 5%; margin-left: 5%;">
          <div class="text-container">

            <h3 style="display: inline-block;">
              Apprendre.

              <br />
              Evoluer.

              <br />
              Réussir.

            </h3>

            <h4 style="display: inline-block; margin-top: 10%;">
              <span class="algiers-text">ALGIERS</span> TECH SUMMER SCHOOL
            </h4>
            <v-divider class="my-4" color="white" width="15%"></v-divider>
            <p style="margin-top: 10%;">Le premier programme de formation pluridisciplinaire de haut niveau conçu pour
              accompagner les
              jeunes algériens dans leurs premiers pas vers le monde professionnel.</p>

          </div>
        </v-col>
        <v-col cols="1"></v-col>
        <v-col cols="6" style="margin-top: 5%;">
          <v-row>

            <v-col cols="6" style="margin-top: 20%;">
              <img src="/images/Rectangle image 1.png">
            </v-col>
            <v-col cols="6">
              <img src="/images/Rectangle image 2.png">
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-img>

  </v-card>
</template>

<script>
import { VImg } from 'vuetify/lib'

export default {
  name: 'IndexPage',
  components: {
    VImg
  }
}
</script>

<style>
#algiers-line {
  position: absolute;
  left: 0;
  right: 0;
  margin: auto;
  top: 50%;
  transform: translateY(50%);
  width: 10%;
}

#algiers-text {
  position: relative;
}

.text-container {
  color: #fff;
}

.text-container h3 {
  font-family: 'Montserrat semibold', sans-serif;
  font-size: 2.5rem;
}

.text-container h4 {
  font-family: 'Montserrat bold', sans-serif;
  font-size: 2rem;
}

* {
  font-family: 'Montserrat', sans-serif;

  /* change this to the color you want your text to be */
}

.background-image-container {
  background-image: url("/images/Background-Polygon.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center center;
}
</style>
