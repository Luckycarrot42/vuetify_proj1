<template>
  <v-app>
    <v-app-bar app color="info" dark>
      <v-toolbar-title>Eductecno</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn to="/home" text>Home</v-btn>
      <v-btn to="/" text>Login</v-btn>
    </v-app-bar>
    <v-content>
      <router-view></router-view>
    </v-content>
    <v-card height="150">
      <v-footer
        absolute
        class="font-weight-medium">
        <v-col
          class="text-center"
          cols="12">
          {{ new Date().getFullYear() }} — <strong>Educamp</strong>
        </v-col>
      </v-footer>
    </v-card>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
  }),
};
</script>
