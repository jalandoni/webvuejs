<template>
  <v-card
    hover
    height="500"
    width="200"
    
  >
    <v-navigation-drawer
      absolute
      src="https://t4.ftcdn.net/jpg/02/91/29/11/240_F_291291138_nN2lKbL798fhCGFzLcpgHa1kVy1xvh3Y.jpg"
      width="100%"
      permanent
      left
    >
    <template v-slot:prepend>
        <v-list-item two-line>
          <v-list-item-avatar>
            <img src="https://upload.wikimedia.org/wikipedia/commons/7/70/User_icon_BLACK-01.png">
          </v-list-item-avatar>

          <v-list-item-content>
            <v-list-item-title>Admin</v-list-item-title>
            <v-list-item-subtitle>Logged In</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </template>
       <v-divider></v-divider>
      <v-list dense>
         <router-link to='/about'>Dashboard</router-link><br>
         <router-link to='/about'>Schedules</router-link><br>
      </v-list>
    </v-navigation-drawer>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
    
    }),
  }
</script>