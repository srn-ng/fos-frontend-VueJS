<template>
    <v-card style="margin-top: -20px" class="pb-5" fluid elevation="0">
        <div>
            <div style=" margin-top: 5%; margin-left: 35%;">
                <h4 style="font-size: 2rem; color: #046380; font-family: 'Montserrat';">Nous contacter</h4>
                <v-divider class="my-4" color="#046380" width="5%"></v-divider>
            </div>
            <div style="background-color: #046380; width:100%; min-height: 400px; margin-top: 5%;">
                <v-row fluid class="outerdiv">

                    <v-col cols="2" class="text-center">
                        <p style="color:white; font-family: 'Montserrat'">Nous sommes là pour répondre à toutes vos
                            questions et recevoir tous vos commentaires!</p>
                    </v-col>
                    <v-col cols="1">

                    </v-col>
                    <v-col cols="6">
                        <v-form>
                            <v-container>
                                <v-row>
                                    <v-col cols="6">
                                        <v-text-field label="Nom" hide-details class="input-field"></v-text-field>
                                    </v-col>
                                    <v-col cols="6">
                                        <v-text-field label="Prénom" hide-details class="input-field"></v-text-field>
                                    </v-col>
                                </v-row>
                                <v-row>
                                    <v-col cols="6">
                                        <v-text-field label="Addresse mail" hide-details class="input-field"></v-text-field>
                                    </v-col>
                                    <v-col cols="6">
                                        <v-text-field label="Téléphone" hide-details class="input-field"></v-text-field>
                                    </v-col>
                                </v-row>
                                <v-row>
                                    <v-col>
                                        <v-textarea background-color="white" label="Message" outlined></v-textarea>
                                    </v-col>
                                </v-row>
                                <v-row>
                                    <v-col>
                                        <button color="primary" dark>Submit</button>
                                    </v-col>
                                </v-row>
                            </v-container>
                        </v-form>
                    </v-col>
                </v-row>
            </div>
            <div class="div-btn">
                <v-btn class="contact">
                    rejoindre programme
                </v-btn>
            </div>
        </div>
    </v-card>
</template>
<style>
.v-col {
    display: flex;
    justify-content: center;
    align-items: center;
}

.outerdiv {
    display: flex;
    justify-content: center;
    align-items: center;
}

.input-field {
    background-color: white;
    border: 1px solid #ccc;
    border-radius: 5px;
    padding: 5px;
    margin-bottom: 10px;
    max-height: 40px;
    height: 40px;
}

.contact {
    width: 380px !important;
    height: 70px !important;
    background-color: #046380 !important;
    color: white !important;
    border-radius: 10px;
}

.div-btn{
    height: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>