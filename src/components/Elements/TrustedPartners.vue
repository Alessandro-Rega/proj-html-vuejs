<template>
  <section>
    <span>Trusted Partners</span>
    <hr>
    <p>Lorem ipsum dolor sit amet. consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua ut enim ad minim veniam.</p>
    <div class="immagini">
        <img src="../../assets/img/estate.png" alt="realestate">
        <img src="../../assets/img/secure.png" alt="securehouse">
        <img src="../../assets/img/forest.png" alt="foresthouse">
        <img src="../../assets/img/market.png" alt="realestatemarket">
        <img src="../../assets/img/food.png" alt="foodhouse">
    </div>
  </section>
</template>

<script>
export default {
    name: 'TrustedPartners',
}
</script>

<style lang="scss" scoped>
// Importazione variabili
@import "../../assets/style/variables.scss";

section{
    padding-top: 100px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding-bottom: 50px;

    span{
        color: $scritta-nero;
        font-size: 35px;
    }

    hr{
        width: 12%;
        border: none;
        border-top: 2px solid $giallo;
        margin: 20px 0 30px 0;
    }

    p{
        width: 48%;
        text-align: center;
        line-height: 30px;
        color: $scritta-grigio;
    }
}

.immagini{
    margin: 45px 0;

    img{
        width: 220px;
        margin: 0 20px;
    }
}
</style>