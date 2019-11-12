<template>

    <v-row>
      <v-col cols ='12'>
        <img  :src="image" rounded="circle" />
         <p>{{info}}</p>
         <p>{{des}}</p>
      </v-col>
      <v-col cols='12'>
          <h2>{{name}}</h2>
      </v-col>
    </v-row>


</template>



<script>
export default {
  props: {
    info:String,
    image: String,
    name: String,
    des:String
  }
};
</script>

<style>
p, h2 {
  color: white;
}







</style>