<template>
  <v-app>
    <v-toolbar fixed app class="secondary px-3" dark>
      <v-spacer></v-spacer>
      <v-toolbar-items>
        <v-btn flat :to="{name: 'Home'}">Home</v-btn>
        <v-btn flat :to="{name: 'Login'}">Login</v-btn>
        <v-btn flat :to="{name: 'components.list'}">Components</v-btn>
        <v-btn flat :to="{name: 'Popup'}">Popup</v-btn>
        <v-btn flat :to="{name: 'Animation'}">Animation</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-content>
      <v-container fluid>
        <router-view />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
