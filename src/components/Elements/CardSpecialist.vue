<template>
  <section>
      <div class="card" v-for="card in cardList" :key="card">
        <div class="img">
            <i :class="card.immagine"></i>
        </div>
        <h3>{{card.nome}}</h3>
        <p>{{card.testo}}</p>
      </div>
  </section>
</template>

<script>
export default {
    name: 'CardSpecialist',
    props:{
        cardList: Object,
    }
}
</script>

<style lang="scss" scoped>
// Importazione variabili
@import "../../assets/style/variables.scss";

section{
    display: flex;
    justify-content: space-between;
    margin: 0 100px;
    margin-bottom: 100px;
}

.card{
    width: 400px;
    background-color: #f5f5f5;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    border-radius: 0.7em;
}

.img{
    display: inline-block;
    color: $scritta-grigio;
    border: 1px solid $scritta-grigio;
    border-radius: 2em;
    margin: 25px 0 15px 0;

    i{
        padding: 0.8em 0.8em;
        font-size: 25px;
    }
}

h3{
    color: $scritta-nero;
    font-weight: 500;
    font-size: 30px;
    margin-bottom: 10px;
}

p{
    text-align: center;
    line-height: 30px;
    color: $scritta-grigio;
    padding-bottom: 40px;
}
</style>