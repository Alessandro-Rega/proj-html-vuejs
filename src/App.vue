<template>
  <div id="app">
    <Header v-bind:vociMenu="vociMenu"/>
  </div>
</template>

<script>

import Header from "./components/Macro/Header.vue"; 

export default {
  name: 'App',
  components: {
    Header,
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
