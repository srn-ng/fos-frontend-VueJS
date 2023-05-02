<template>
  <v-card style="margin-top: -20px" class="pb-5" fluid elevation="0">
    <v-img src="/images/Background-Polygon-3.png" cover>
      <div>
        <div style="margin-left: 35%; margin-top:5%">
          <h4 style="font-size: 2rem; color: #046380; font-family: 'Montserrat';">Calendrier</h4>
          <v-divider class="my-4" color="#046380" width="5%"></v-divider>
        </div>

        <div
          style="
            margin-top: 5%;
            margin-left: 35%;
            margin-right: 15%;
            text-align: justify;
          "
        >
          <p class="description">
            La première édition de ce programme est programmée sur une durée de
            8 semaines à compter du xx xx 2023 jusqu’au xx xx 2023.
          </p>
        </div>
        <div style="margin-top: 5%; margin-left: 35%; margin-right:15%">
          <v-simple-table height="300px">
            <template v-slot:default>
              <tbody>
                <tr v-for="item in formations" :key="item.titre" class="text-center">
                  <td >
                    <div :style="{ 'padding': '10px 0px 10px 0px ', 'backgroundColor': '#D9D9D9', 'color':'white', 'font-weight':'bold', 'width':'100%'}">
                        {{ item.date }}
                    </div>
                 </td>
                  <td style="color:#046380" >{{ item.titre }}</td>
                </tr>
              </tbody>
            </template>
          </v-simple-table>
        </div>
      </div>
    </v-img>
  </v-card>
</template>

<script>
export default {
    data(){
        return{
            formations: [
                {
                    date: '28 Mai 2023',
                    titre: 'Début de la formation'
                },
                {
                    date: '11 Juin 2023',
                    titre: 'Début des stages pratiques'
                },
                {
                    date: '18 Juin 2023',
                    titre: 'Début des conférences'
                },
                {
                    date: '03 Septembre 2023',
                    titre: 'Cérémonie de clôture'
                },
            ] 
        }
    }


}
</script>

<style>
.description{
    color:#6E6B80;
}
</style>