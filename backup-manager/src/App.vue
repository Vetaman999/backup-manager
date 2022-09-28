<template>
  <v-app>
    <v-app-bar app color="primary" dark>

      <v-btn :to="{path:'/'}" text>
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
