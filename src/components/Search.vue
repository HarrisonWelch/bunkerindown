<template>
  <v-layout>
    <link href="https://fonts.googleapis.com/css?family=Material+Icons" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.0.0-beta/css/bootstrap.min.css">
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css">
    <v-navigation-drawer permanent>
    </v-navigation-drawer>
    <v-toolbar>
      <v-toolbar-side-icon></v-toolbar-side-icon>
      <v-toolbar-title>Bunkerin' Down</v-toolbar-title>
      <v-spacer></v-spacer>
      <!-- <v-toolbar-items class="hidden-sm-and-down">
        <v-btn flat>Link One</v-btn>
        <v-btn flat>Link Two</v-btn>
        <v-btn flat>Link Three</v-btn>  
      </v-toolbar-items> -->
    </v-toolbar>
    <!-- <v-card> -->
      <div id="map" class="map"></div>
    <!-- </v-card> -->
  </v-layout>
  
<!-- <script src="https://cdnjs.cloudflare.com/ajax/libs/vue/2.3.4/vue.min.js"></script>
<script src="https://unpkg.com/leaflet@1.2.0/dist/leaflet.js"></script> -->
</template>


<script>
import L from "leaflet"

export default {
  name: 'Search',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      map: null,
      tileLayer: null
    }
  },
  methods: {
    goToSearch () {
      console.log('goToSearch')
    }
  },
  mounted: function(){
    this.map = L.map('map').setView([51.505, -0.09], 13);

    this.tileLayer = L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreet Map</a> contributors'
    })

    this.tileLayer.addTo(this.map);

    // L.marker([51.5, -0.09]).addTo(this.map)
    // .bindPopup('A pretty CSS3 popup.<br> Easily customizable.')
    // .openPopup();
  }
}
</script>

<style>
.map{
  height: 600px;
}
</style>
