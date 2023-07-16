<template>
  <div class="pb-5 h-100">
    <v-row justify="center" class="pb-5">
      <v-col cols="10" md="4" class="d-flex align-center">
        <div class="text-container">
          <h4 style="display: inline-block">
            Apprendre.

            <br />
            Evoluer.

            <br />
            Réussir.
          </h4>

          <h3 class="my-5">The Finish Off SCHOOL</h3>
          <v-divider class="my-4" color="white" width="15%"></v-divider>
          <p style="margin-top: 10%">
            Le premier programme de formation pluridisciplinaire de haut niveau
            conçu pour accompagner les jeunes algériens dans leurs premiers pas
            vers le monde professionnel.
          </p>
        </div>
      </v-col>
      <!-- <v-col cols="1"></v-col> -->
      <v-col cols="10" md="4" style="margin-top: 5%">
        <v-row>
          <v-col cols="6" style="margin-top: 20%">
            <img
              src="/images/Rectangle image 1.png"
              v-if="$vuetify.breakpoint.lgAndUp"
              style="margin-left: -10%"
            />
          </v-col>
          <v-col cols="6">
            <img
              src="/images/Rectangle image 2.png"
              v-if="$vuetify.breakpoint.lgAndUp"
            />
          </v-col>
        </v-row>
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
@media only screen and (max-width: 600px) {
  /* Apply style to h3 with class 'small-screen' */
  .small-screen {
    font-size: 1.5rem;
    /* Add any other styles you want to apply to h3 on small screens */
  }
}

@media only screen and (min-width: 601px) {
  /* Apply style to h3 with class 'large-screen' */
  .large-screen {
    font-size: 2.5rem;
    display: inline-block;
    text-align: center;
    /* Add any other styles you want to apply to h3 on large screens */
  }
}

#algiers-line {
  position: absolute;
  left: 0;
  right: 0;
  margin: auto;
  top: 50%;
  transform: translateY(50%);
  width: 10%;
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
  font-size: 1.5rem;
}

* {
  font-family: 'Montserrat', sans-serif;
}

.background-image-container {
  background-image: url('/images/Background-Polygon.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center center;
}
</style>
