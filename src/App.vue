<template>
  <v-app id="app" dark>
    <v-app-bar dark fixed flat hide-on-scroll color="transparent">
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
        <v-toolbar-title>취운화</v-toolbar-title>
        <v-spacer />
        <v-btn icon><v-icon>mdi-magnify</v-icon></v-btn>
    </v-app-bar>

    <abouts />
    <v-spacer />
    <slides />
    <v-spacer />
    <orders />

    <v-footer absolute padless>
        <v-card flat tile width="100%">
            <v-card-title>(c) 취운화</v-card-title>
            <v-card-text>since 2019</v-card-text>


        </v-card>
    </v-footer>
  </v-app>
</template>

<script>
import abouts from './components/Abouts'
import slides from './components/Slides'
import orders from './components/Orders'

export default {
  name: 'app',
  components: {
    abouts,
    slides,
    orders,
  },
  data() {
    return {
      
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
