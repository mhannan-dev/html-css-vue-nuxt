<template>
  <v-app>
    <AppHeader/>
    <v-main>
      <HeroArea/>
      <AboutUs/>
      <Portfolio/>
    </v-main>
  </v-app>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import HeroArea from './components/HeroArea.vue'
import AboutUs from './components/AboutUs.vue'
import Portfolio from './components/PortfolioSection.vue'
export default {
  name: "App",
  components: {AppHeader, HeroArea, AboutUs, Portfolio}
}
</script>
<style lang="css" scoped>
</style>