<template>
  <v-app>
    <AppHeader />
    <v-main>
      <HeroArea />
      <AboutUs />
      <Portfolio />
      <Project />
      <Gallery />
      <Contact />
      <Footer/>
    </v-main>
  </v-app>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import HeroArea from "./components/HeroArea.vue";
import AboutUs from "./components/AboutUs.vue";
import Portfolio from "./components/PortfolioSection.vue";
import Project from "./components/ProjectSection.vue";
import Gallery from "./components/GallerySection.vue";
import Contact from "./components/ContactUs.vue";
import Footer from "./components/FooterPart.vue";
export default {
  name: "App",
  components: {
    AppHeader,
    HeroArea,
    AboutUs,
    Portfolio,
    Project,
    Gallery,
    Contact,
    Footer,
  },
};
</script>
<style lang="css" scoped></style>
