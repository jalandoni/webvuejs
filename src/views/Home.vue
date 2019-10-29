<template>
  <div class="home">
    <div class="home">
    <dev v-bind:picture = "require('@/assets/home.png')" v-bind:name="'WeOrg!'"></dev>
  </div>
  </div>
</template>

<script>
import dev from "@/components/developers";
export default {
  components:{
    dev
  }
};
</script>
