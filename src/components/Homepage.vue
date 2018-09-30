<template>
  <div class="homepage">
    <link href="https://cdn.jsdelivr.net/npm/vuetify/dist/vuetify.min.css" rel="stylesheet">
    <v-content>

      <svg id="title" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1920 179.17"><title>bannerinline</title><g id="Mask"><polygon points="1920 0 1920 54.59 1899.96 0 1920 0" style="fill:#ed4636"/><polygon points="22.41 0 0 61.03 0 0 22.41 0" style="fill:#ed4636"/><polygon points="109.77 0 52.51 156 0 156 0 153.9 56.49 0 109.77 0" style="fill:#ed4636"/><polygon points="198.77 0 141.51 156 86.59 156 143.86 0 198.77 0" style="fill:#ed4636"/><polygon points="288.41 0 231.14 156 175.59 156 232.86 0 288.41 0" style="fill:#ed4636"/><polygon points="375.77 0 318.51 156 265.23 156 322.49 0 375.77 0" style="fill:#ed4636"/><polygon points="464.77 0 407.51 156 352.59 156 409.86 0 464.77 0" style="fill:#ed4636"/><polygon points="1480.77 156 441.59 156 498.86 0 1423.51 0 1480.77 156" style="fill:#ed4636"/><polygon points="1569.77 156 1514.86 156 1457.59 0 1512.51 0 1569.77 156" style="fill:#ed4636"/><polygon points="1657.14 156 1603.86 156 1546.59 0 1599.87 0 1657.14 156" style="fill:#ed4636"/><polygon points="1746.77 156 1691.23 156 1633.96 0 1689.51 0 1746.77 156" style="fill:#ed4636"/><polygon points="1835.77 156 1780.86 156 1723.59 0 1778.51 0 1835.77 156" style="fill:#ed4636"/><polygon points="1920 147.45 1920 156 1869.86 156 1812.59 0 1865.87 0 1920 147.45" style="fill:#ed4636"/><line x1="1812.59" x2="1778.51" style="fill:#ed4636"/></g><g id="Text"><text transform="translate(585.64 124.89)" style="font-size:120px;fill:#ede6de;font-family:Impact, Impact">Bunkerin’ Down</text></g></svg>

      <v-container>
        <p class="text-xs-center center_vert"><br><br>
          <!-- ed4636 -->
          <v-btn class="text-xs-center wide_button" to="/search">Search</v-btn> <br><br>
          <v-btn class="text-xs-center wide_button">Plan</v-btn> <br><br>
          <v-btn class="text-xs-center wide_button">Review</v-btn> <br><br>
        </p>
      </v-container>
    </v-content>
  </div>
</template>

<script>
export default {
  name: 'Homepage',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    goToSearch () {
      console.log('goToSearch')
    }
  }
}
</script>

<style>
.homepage {
  background-color: #ede6de;
  margin-top: -6%;
  height: 106%;
}
.center_vert {
  /* padding-top: 30%; */
}

.wide_button {
  width: 30%;
}
/* 
.search_button {
  background-color: #ed4636;
  color: ede6de;
} */

#title {
  padding-top: 20%
}
</style>
