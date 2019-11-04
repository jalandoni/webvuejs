<template>
  <div class="about">


      <h1 >Developers</h1>
 

    <developer v-bind:picture = "require('../assets/grace.png')" v-bind:name="'Grace'"></developer>
      
    <developer v-bind:picture = "require('../assets/jess.jpg')" v-bind:name="'Jessa'"></developer>
  
    <developer v-bind:picture = "require('../assets/ivy.png')" v-bind:name="'Ivy'"></developer>

    <developer v-bind:picture= "require('../assets/gen.png')" v-bind:name="'Gen'"></developer>
  
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




