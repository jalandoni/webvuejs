<template>
  <v-app>
    <v-app-bar app>
      <router-link to="/">Home</router-link>|
      <router-link to="/about">About</router-link>
    </v-app-bar>

    <v-content>
      <router-view/>
    </v-content>
  </v-app>
</template>

<script>

export default {
  name: "App",
  data: () => ({
    //
  })
};
</script>
