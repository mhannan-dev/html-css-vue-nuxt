<template>
  <v-app>
    <AppHeader/>
    <v-main>
      <HeroArea/>
      <AboutUs/>
      <Portfolio/>
      <Project/>
    </v-main>
  </v-app>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import HeroArea from './components/HeroArea.vue'
import AboutUs from './components/AboutUs.vue'
import Portfolio from './components/PortfolioSection.vue'
import Project from './components/ProjectSection.vue'
export default {
  name: "App",
  components: {AppHeader, HeroArea, AboutUs, Portfolio, Project}
}
</script>
<style lang="css" scoped>
</style>