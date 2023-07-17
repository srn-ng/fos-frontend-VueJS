<template>
  <div class="container mt-15">
    <v-row justify="center">
      <v-col
        class="contact-info d-flex align-center justify-center p-0 mr-md-n12 mr-lg-n10"
        cols="10"
        md="4"
      >
        <v-card class="px-md-5 py-md-15" color="rgba(4, 99, 128)">
          <v-card-title class="white-title">Contact info</v-card-title>
          <v-card-text>
            <ul>
              <li>
                <v-icon color="white" class="mr-1"> mdi-map-marker </v-icon>
                <span>137 ter Bd Colonel Krim Belkacem, Algiers</span>
              </li>
              <li>
                <v-icon color="white" class="mr-1"> mdi-mail </v-icon>
                <span>contact@finishoffschool.com</span>
              </li>
            </ul>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="10" md="5" class="ml-md-n5">
        <v-card class="px-7 px-md-15 py-md-10" color="rgb(219, 218, 218)">
          <v-card-title class="blue-title">Contactez-nous</v-card-title>
          <v-card-text>
            <v-form v-model="valid">
              <v-text-field
                v-model="firstname"
                :rules="nameRules"
                :counter="10"
                label="Nom"
                required
              ></v-text-field>

              <v-text-field
                v-model="lastname"
                :rules="nameRules"
                :counter="10"
                label="Prénom"
                required
              ></v-text-field>

              <v-text-field
                v-model="email"
                :rules="emailRules"
                label="E-mail"
                required
              ></v-text-field>

              <v-textarea
                v-model="message"
                variant="filled"
                auto-grow
                label="Message"
                rows="4"
                row-height="30"
                shaped
                required
              ></v-textarea>

              <v-btn
                :disabled="!valid"
                style="
                  background-color: #046380 !important;
                  color: #fff !important;
                "
                class="mr-4"
                @click="validate"
              >
                Envoyer
              </v-btn>
            </v-form>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>
<script>
export default {
  data: () => ({
    valid: false,
    firstname: '',

    lastname: '',
    nameRules: [
      (v) => !!v || 'Name is required',
      (v) => v.length <= 10 || 'Name must be less than 10 characters',
    ],
    email: '',
    emailRules: [
      (v) => !!v || 'E-mail is required',
      (v) => /.+@.+/.test(v) || 'E-mail must be valid',
    ],
    message: '',
  }),
  methods: {
    validate: () => ({}),
  },
}
</script>

<style scoped>
.blue-title {
  color: #046380;
  font-weight: bold;
}

.white-title {
  color: #fff;
  font-weight: bold;
}
.contact-form {
  padding: 5rem;
}
.contact-info {
  z-index: 1000;
}
ul {
  color: white;
}
li {
  position: relative;
  list-style: none;
  display: flex;
  margin: 25px 0;
  cursor: pointer;
  align-items: flex-start;
  color: white;
}
</style>