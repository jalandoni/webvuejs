<template>
  <div class="about">
    <dev v-bind:picture = "require('@/assets/princess.png')" v-bind:name="'Princess'"></dev>
    <dev v-bind:picture = "require('@/assets/lorly.png')" v-bind:name="'Lorly'"></dev>
    <dev v-bind:picture = "require('@/assets/mellyne.png')" v-bind:name="'Mellyne'"></dev>
    <dev v-bind:picture = "require('@/assets/jacky.png')" v-bind:name="'Jakeniel'"></dev>
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




