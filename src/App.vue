<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-toolbar-title text-h5 font-weight-bold >Gestor de Backups</v-toolbar-title>
      <v-btn class="pa-2 ml-auto" :to="{path:'/'}" text>
        <v-icon>
          mdi-exit-run
        </v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
