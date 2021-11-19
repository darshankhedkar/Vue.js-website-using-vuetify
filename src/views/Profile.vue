<template>
  <v-card height="100%">
<div>
 
        <v-list-item two-line>
          <v-list-item-avatar>
            <img src="https://pbs.twimg.com/profile_images/1383807203295911948/jn-nmBon.jpg">
          </v-list-item-avatar>

          <v-list-item-content>
            <v-list-item-title>Darshan</v-list-item-title>
            <v-list-item-subtitle>Logged In</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      

      <v-divider></v-divider>

      <v-list >
        <v-list-item
          v-for="item in items"
          :key="item.title"
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
</div>

    
  </v-card>
</template>
<script>
  export default {
    data () {
      return {
        items: [
          { title: 'Home', icon: 'mdi-home-city' },
          { title: 'My Account', icon: 'mdi-account' },
          { title: 'Users', icon: 'mdi-account-group-outline' },
        ],
      }
    },
  }
</script>