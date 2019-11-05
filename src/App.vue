<template>
<center>
<div id="navigate">
 <div id="app">
   <div class="card">
     <NavBar/>
   </div>
   <div class="content">
     <router-view/>
     </div>
 </div>
 </div>
 </center>
</template>

<script>
import NavBar from '@/components/headerBar.vue'
export default {
 name: 'home',
 components: {
   NavBar
 }
}
</script>
<style>



.card{
  padding-top:25px;
  padding-bottom:25px;
}




#navigate a {
  font-weight: bold;
  color: black;
}

#navigate a.router-link-exact-active {
  color: blue;
}


</style>



