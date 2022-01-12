<template>
  <div id="app">
    <Header v-bind:vociMenu="vociMenu"/>
    <Hero/>
  </div>
</template>

<script>

import Header from "./components/Macro/Header.vue";
import Hero from "./components/Macro/Hero.vue"; 

export default {
  name: 'App',
  components: {
    Header,
    Hero,
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
