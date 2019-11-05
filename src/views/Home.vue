<template>
  <div class="home">
    <div class="home">
    <card>
    <developersProfile v-bind:image = "require('../assets/logo.png')" v-bind:name="'Tootbook'"></developersProfile>
    <h4>Provide list of dental services</h4>
    <v-col cols ='12'>
    <h5>The services provided include teeth extraction, cosmetic crown, botox, flux surgery and many more.This can be attained through this easy and fast means of booking throungh a fixed set of schedule using toothbook</h5>
    </v-col>
    </card>
  </div>
  </div>
</template>


<script>
import developersProfile from "../components/developersProfile";
export default {
  components:{
    developersProfile
  }
};
</script>

<style>
h5{
	color: black;
	margin-left:25%;
	margin-right:25%

}
</style>
