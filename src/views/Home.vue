<template>
  <div class="home">
    <div class="home">
      <app-sidebar></app-sidebar>
    
    <div class="row">
      <div class="col-md-6">

    <developersProfile v-bind:image = "require('../assets/toothlogo1.png')" v-bind:name="'Tootbook'"></developersProfile>
 </div>

    <div class="col-md-5">
        <div>
    <b-table striped hover :items="items" :fields="fields"></b-table>
  </div>
      
        </div>
  </div>
  </div>
  </div>
</template>


<script>
import developersProfile from "../components/developersProfile";
import SideBar from '../components/sideBar.vue'
export default {
  components:{
    developersProfile,
    'app-sidebar':SideBar
  },
   data() {
      return {
        // Note 'isActive' is left out and will not appear in the rendered table
        fields: [
          {
            key: 'name',
            variant: 'primary'

          },
          {
            key: 'number',
            variant: 'primary'

          },
          {
            key: 'email',
            label: 'Email Address',
            variant: 'primary'
          },
          {
            key: 'date',
            label: 'Date',
            variant: 'primary'
          },
          {
            key: 'service',
            label: 'Service',
            variant: 'primary'
          },
          {
            key: 'status',
            label: 'Status',
            variant: 'primary'
          }
        ],
        items: [
          { status: 'done', service: 'cleaning', date: 'jan',email:'@gmail',number:'09',name:'jessa' },
        ]
      }
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
