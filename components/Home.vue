<template>
  <div class="home">
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
              Le premier programme de formation pluridisciplinaire de haut
              niveau conçu pour accompagner les jeunes algériens dans leurs
              premiers pas vers le monde professionnel.
            </p>
          </div>
        </v-col>
        <!-- <v-col cols="1"></v-col> -->
        <v-col cols="10" md="4" style="margin-top: 5%">
          <v-row>
            <v-col cols="6" style="margin-top: 20%">
              <v-card rounded>
                <v-img src="/images/Rectangle image 1.jpg"></v-img>
              </v-card>
            </v-col>
            <v-col cols="6">
              <v-card rounded>
                <v-img src="/images/Rectangle image 2.jpg"></v-img>
              </v-card>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </div>
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

<style scoped>
.home {
  clip-path: polygon(9% 0, 100% 0, 100% 90%, 90% 100%, 0 100%, 0 9%);
  background-color: rgba(4, 99, 128);
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
</style>
