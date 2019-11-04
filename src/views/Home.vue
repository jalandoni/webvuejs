<template>
  <div class="home">
    <div class="home">
    <dev v-bind:picture = "require('../assets/logo.png')" v-bind:name="'Tootbook'"></dev>
  </div>
  </div>
</template>



<script>
import dev from "../components/developersProfile";
export default {
  components:{
    dev
  }
};
</script>
