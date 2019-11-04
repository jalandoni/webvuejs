<template>
  <v-app>
    <center>
    <div id="navigate">
    <v-app-bar app>
     <div v-bind:style="styleObject">
      <router-link to="/" id="home">Home</router-link>  |
      </div>
      <router-link to="/about">About</router-link>
    </v-app-bar>
</div>
    <v-content>
      <router-view/>
    </v-content>
    </center>
  </v-app>
</template>

<script>

export default {
  name: "App",
  data: () => ({
    styleObject: {
    color: 'red',

  }
  })
};

</script>
<style>


#nav {
  padding: px;
}

hover #navigate {
  color:yellow;
}

#navigate a {
  font-weight: bold;
  color: black;
}

#navigate a.router-link-exact-active {
  color: blue;
}

/* *{
      box-sizing:border-box;
      margin:0;
  } */
</style>



