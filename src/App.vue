<template>
  <v-app>
    <HeaderComp />
    <v-main>
      <HeroComp />
      <AboutmeComp />
      <PortfolioComp />
      <Projects />
      <GalleryComp />
      <ContactusComp />

      <FooterComp />
    </v-main>
  </v-app>
</template>

<script>
import AboutmeComp from "./components/AboutmeComp.vue";
import ContactusComp from "./components/ContactusComp.vue";
import FooterComp from "./components/FooterComp.vue";
import GalleryComp from "./components/GalleryComp.vue";
import HeaderComp from "./components/HeaderComp.vue";
import HeroComp from "./components/HeroComp.vue";
import PortfolioComp from "./components/PortfolioComp.vue";
import Projects from "./components/Projects.vue";
export default {
  name: "App",
  components: {
    HeaderComp,
    HeroComp,
    AboutmeComp,
    PortfolioComp,
    Projects,
    GalleryComp,
    ContactusComp,
    FooterComp,
  },
};
</script>
