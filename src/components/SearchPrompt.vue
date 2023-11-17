<template>
  <!-- <v-layout class="rounded rounded-md"> -->

    <v-container     class=" pa-6">
        <v-row justify="center">
            <v-col cols="auto" sm="8">
                <v-textarea
                label="Votre recherche"
                auto-grow
                variant="outlined"
                rows="3"
                row-height="15"
                ></v-textarea>
            </v-col> 
            <v-col align-self="end" cols="auto" sm="2">
                <v-btn>
                    Rechercher
                </v-btn>
            </v-col>
        </v-row>
        <v-spacer></v-spacer>
        <v-row align="center" justify="center">
            <v-col
                v-for="(keywords, i) in keywords"
                :key="i"
                cols="auto" 

            >
                <v-card
                class="mx-auto"
                max-width="344"
                :variant="elevated"
                >
                <v-card-item>
                    <div>
                    <div class="text-overline mb-1">
                        Mots-clé
                    </div>
                    <div class="text-h6 mb-1 text-center text-capitalize" justify="center">
                        {{ keywords }}
                    </div>
                    <div class="text-caption">Greyhound divisely hello coldly fonwderfully</div>
                    </div>
                </v-card-item>

                <v-card-actions>
                    <v-btn>
                    Rechercher les offres
                    </v-btn>
                </v-card-actions>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
  <!-- </v-layout> -->
</template>
  
  <script setup>
    const keywords = ['secrétaire', 'mannutentionnaire', 'tonal', 'outlined']
  </script>