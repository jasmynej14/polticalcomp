<template>
  <v-app>
    <v-app-bar color="#ecf0f1" dense>
      <v-app-bar-title>Political Compatibility</v-app-bar-title>
    </v-app-bar>
    <navigation></navigation>
  </v-app>
</template>

<script>


import Navigation from './components/Navigation.vue';
export default {
  
  name: 'App',

  components: {
    Navigation
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
