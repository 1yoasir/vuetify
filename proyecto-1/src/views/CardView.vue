<template>
    <v-container grid-list-md>
        <v-layout row wrap>
            <v-flex xs12 sm6>
                <v-card>
                    <v-img src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"></v-img>
                    <v-card-title>
                        <h2>Lorem, ipsum dolor.</h2>
                    </v-card-title>
                    <v-card-text>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est sed illo porro magni, nesciunt esse deleniti, harum accusantium voluptatem illum numquam natus sit dolore quis perspiciatis, atque ipsam optio consectetur.</p>
                    </v-card-text>
                    <v-card-actions>
                        <v-btn color="info" text @click="dialog = true">Acción</v-btn>
                    </v-card-actions>
                </v-card>
            </v-flex>

            <v-flex xs12 sm6>
                <v-card>
                    <v-img src="https://cdn.vuetifyjs.com/images/cards/docks.jpg">
                        <v-container>
                            <v-layout>
                                <v-flex>
                                    <v-card-title class="headline white--text">Lorem, ipsum dolor.</v-card-title>
                                </v-flex>
                            </v-layout>
                        </v-container>
                    </v-img>
                    <v-card-title>
                        <h2>Lorem, ipsum dolor.</h2>
                    </v-card-title>
                    <v-card-text>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est sed illo porro magni, nesciunt esse deleniti, harum accusantium voluptatem illum numquam natus sit dolore quis perspiciatis, atque ipsam optio consectetur.</p>
                    </v-card-text>
                    <v-card-actions>
                        <v-btn color="info" text @click="dialog = true">Acción</v-btn>
                    </v-card-actions>
                </v-card>
            </v-flex>
        </v-layout>

    <!-- Dialog -->

    <v-dialog v-model="dialog" width="500" persistent>
        <v-card>
            <v-card-title>Este es el título</v-card-title>
            <v-card-text>Lorem, ipsum dolor sit amet consectetur adipisicing elit. 
                Soluta necessitatibus, eaque libero aperiam consequuntur quaerat laborum quos 
                distinctio obcaecati quam eveniet ipsa ipsam expedita porro repellat amet deserunt 
                esse quo.
            </v-card-text>
            <v-divider></v-divider>
            <v-card-actions>
                <v-btn @click="dialog = false">Cerrar</v-btn>
            </v-card-actions>
        </v-card>
    </v-dialog>

    <!-- Fin dialog -->
    </v-container>
</template>

<script>
export default {
    data:() => {
        return ({
            dialog: false
        })
    }
}
</script>