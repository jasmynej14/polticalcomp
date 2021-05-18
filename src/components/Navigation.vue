<template>
    <v-app>
        <v-navigation-drawer  permanent>
      <v-list
        dense
        nav
      >
        <v-list-item
          v-for="item in items"
          :key="item.title"
          link
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
   
    <v-bottom-navigation></v-bottom-navigation>
    </v-app>
</template>

<script>
    export default {
  name: 'Navigation',

  components: {
    
  },

  data () {
      return {
        items: [
          { title: 'Home', icon: 'mdi-home' },
          { title: 'Profile', icon: 'mdi-view-dashboard' },
          { title: 'Take the Test', icon: 'mdi-newspaper' },
          { title: 'Map', icon: 'mdi-google-maps' },
        ],
        right: null,
      }
    }
  
};
</script>