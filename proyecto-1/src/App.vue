<template>
  <v-app>
    <v-card class="mb-5" app>
      <v-app-bar app class="primary">
        <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
        <v-toolbar-title>Vuetify</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn class="success">Ingreso</v-btn>
        <v-btn class="error">Salir</v-btn>
      </v-app-bar>
      <v-navigation-drawer app v-model="drawer" temporary dark>
        <v-layout mt-4 align-center column>
          <v-flex>
            <v-avatar>
              <img src="https://randomuser.me/api/portraits/men/85.jpg" alt="" srcset="">
            </v-avatar>
          </v-flex>

          <v-flex>
            <p class="white--text mt-3 headline">Juanito Pérez</p>
          </v-flex>
        </v-layout>

        <v-layout column>
          <v-flex class="mx-3">
            <v-btn color="success" block class="mb-3" :to="{name:'home'}">Home</v-btn>
            <v-btn color="success" block :to="{name:'tareas'}">Lista de Tareas</v-btn>
          </v-flex>
        </v-layout>
      </v-navigation-drawer>
    </v-card>
    
  
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: ()=>{
    return{
      drawer: true
    }
  },
};
</script>
