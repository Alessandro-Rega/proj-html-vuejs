<template>
  <div class="hero">
      <h1>building inspiring spaces</h1>
      <p>We Build inspiring Residential & Commercial Spaces</p>
      <div>
        <button class="btn">explore recent work</button>
        <button class="btn">get a quote today</button>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Hero',
    components: {
    },
}
</script>

<style lang="scss" scoped>
// Importazione variabili
@import "../../assets/style/variables.scss";

.hero{
    // Sezione sfondo
    width: 100%;
    height: 790px;
    background-image: url("../../assets/img/jumbotron.png");
    background-size: 100%;
    background-repeat: no-repeat;
    // --
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    p{
        font-size: 20px;
        color: $giallo;
        margin: 20px 0;
        font-weight: bold;
    }

    button{
        font-size: 18px;
        padding: 18px 50px;
        margin: 0 20px;
    }

    button:first-of-type{
        background-color: $nero;
        color: $bianco;
    }

    button:last-of-type{
        background-color: $giallo;
        color: $nero;
    }
}
</style>