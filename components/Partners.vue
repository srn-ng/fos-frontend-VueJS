<template>
  <div class="container mt-15">
    <div>
      <div class="d-flex justify-center">
        <div class="mb-5">
          <h4 style="font-size: 2rem; color: #046380">Nos partenaires</h4>
          <v-divider class="my-4" color="#046380" width="25%"></v-divider>
        </div>
      </div>
      <v-row class="my-row" justify="center" align-items="center">
        <v-col cols="2" class="my-col">
          <div class="partenaire"></div>
        </v-col>
        <v-col cols="2" class="my-col">
          <div class="partenaire"></div>
        </v-col>
        <v-col cols="2" class="my-col">
          <div class="partenaire"></div>
        </v-col>
        <v-col cols="2" class="my-col">
          <div class="partenaire"></div>
        </v-col>
        <v-col cols="2" class="my-col">
          <div class="partenaire"></div>
        </v-col>
      </v-row>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.partenaire {
  background-color: #d9d9d9;
  width: 100px;
  height: 100px;
  border-radius: 50%;
}
</style>