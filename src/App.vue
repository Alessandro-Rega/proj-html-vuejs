<template>
  <div id="app">
    <Header v-bind:vociMenu="vociMenu"/>
    <Hero/>
    <Main/>
  </div>
</template>

<script>

import Header from "./components/Macro/Header.vue";
import Hero from "./components/Macro/Hero.vue"; 
import Main from "./components/Macro/Main.vue"; 

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Main,
  },
  data(){
    return{
      vociMenu: ["Home", "About", "Services", "Work", "Articles",],
    }
  },
}
</script>

<style lang="scss">
@import "./assets/style/global.scss";
</style>
