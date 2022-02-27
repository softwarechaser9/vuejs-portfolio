<template>
  <v-app>
    <Header />
    <v-main>
      <HeroComponent />
      <!-- About us -->
      <Aboutus />
      <!-- Portfolio -->
      <Portfolio/>
      <!-- project -->
      <Project/>
      <!-- Gallery -->
      <Gallery/>
      <!-- Contact -->
      <Contact/>
      <!-- Footer -->
      <Footer/>
    </v-main>
    
  </v-app>
</template>

<script>
import Header from "./components/Header.vue";
import HeroComponent from "./components/HeroComponent.vue";
import Aboutus from "./components/Aboutus.vue";
import Portfolio from "./components/Portfolio.vue";
import Project from "./components/Project.vue";
import Gallery from "./components/gallery.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";
export default {
  name: 'App',
  components: { Header, HeroComponent, Aboutus, Portfolio, Project, Gallery, Contact, Footer },

};
</script>
