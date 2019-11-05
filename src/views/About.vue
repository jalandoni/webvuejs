<template>
  <div class="about">
    <h1 >Developers</h1>

    <b-container fluid class="p-4 bg-dark">

    <b-row>

      <developer v-bind:image = "require('@/assets/grace.png') " 
      v-bind:info="'Project Manager'" v-bind:des="'A dedicated student'" v-bind:name="'Grace'"></developer>

      <developer v-bind:image = "require('@/assets/jess.jpg')" 
      v-bind:info="'Front-end Developer'" v-bind:des="'A courageous student'"  v-bind:name="'Jessa'"></developer>

      <developer v-bind:image= "require('@/assets/ivy.png')"
      v-bind:info="'Back-end Developer'" v-bind:des="'A persistent student'"  v-bind:name="'Ivy'"></developer>

      <developer v-bind:image= "require('@/assets/gen.png')"
      v-bind:info="'Back-end Developer'" v-bind:des="'A hardworking student'" v-bind:name="'Gen'"></developer>

     </b-row>

    </b-container>
  </div>
  </template>

<script>
import developer from "@/components/developersProfile";
export default {
  components:{
    developer
  }
};
</script>




