<template>
  <div id="app">
    <Header v-bind:vociMenu="vociMenu"/>
    <Hero/>
    <Main/>
    <Footer v-bind:contatti="Contatti"/>
  </div>
</template>

<script>

import Header from "./components/Macro/Header.vue";
import Hero from "./components/Macro/Hero.vue"; 
import Main from "./components/Macro/Main.vue"; 
import Footer from "./components/Macro/Footer.vue"; 

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Main,
    Footer,
  },
  data(){
    return{
      vociMenu: ["Home", "About", "Services", "Work", "Articles",],
      Contatti: [
        {
          icona: "fas fa-globe",
          testo: "Corporate Location 1600 Amphittheatre Parkway London WC1 1BA",
        },
        {
          icona: "fas fa-home",
          testo: "Residential Location 9521 Broadsberry Avenue Paddington RC7 9ZA",
        },
        {
          icona: "fas fa-phone",
          testo: "1.800.458.556 / 1.800.532.2112",
        },
        {
          icona: "far fa-envelope",
          testo: "info@your-domain.com",
        },
        {
          icona: "far fa-clock",
          testo: "Monday - Friday: 9:00 AM - 6:00 PM",
        },
        {
          icona: "far fa-clock",
          testo: "Saturday - Sunday: 9:00 AM - 12:00 PM",
        },
      ],
    }
  },
}
</script>

<style lang="scss">
@import "./assets/style/global.scss";
</style>
