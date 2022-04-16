<template>
    <v-container>
        <v-row>
            <v-flex>
                
                <v-btn>Texto</v-btn>
                <v-btn color="primary">Texto</v-btn>
                <v-btn dark color="blue">Texto</v-btn>

                <v-btn text>Sin fondo</v-btn>

                <v-btn color="warning" large>Largo</v-btn>
                <v-btn color="warning" small>Largo</v-btn>
                <v-btn color="warning" small :disabled="false">Largo</v-btn>

                <v-btn color="info" depressed>Botón</v-btn>

                <v-btn>
                    <v-icon>forum</v-icon>
                </v-btn>

                <v-btn color="primary" icon>
                    <v-icon>forum</v-icon>
                </v-btn>

                <v-btn color="primary" fab>
                    <v-icon>forum</v-icon>
                </v-btn>
                <v-btn color="primary" fab small>
                    <v-icon>forum</v-icon>
                </v-btn>
                <v-btn color="primary" fab large>
                    <v-icon>forum</v-icon>
                </v-btn>

                <v-btn color="success">
                    texto
                    <v-icon>forum</v-icon>
                </v-btn>
                <v-btn color="success">
                    texto
                    <v-icon class="ml-2">forum</v-icon>
                </v-btn>
                <v-btn color="success">
                    texto
                    <v-icon right>forum</v-icon>
                </v-btn>
                <v-btn color="success">
                    <v-icon left>forum</v-icon>
                    texto
                </v-btn>

                <v-btn color="success" outlined>
                    <v-icon left>forum</v-icon>
                    texto
                </v-btn>
                
                <v-btn color="success" outlined block rounded>
                    <v-icon left>forum</v-icon>
                    texto
                </v-btn>

                

            </v-flex>
        </v-row>
    </v-container>
</template>

<script>
export default {
    data(){
        return{

        }
    }
}
</script>