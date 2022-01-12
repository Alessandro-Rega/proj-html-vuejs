<template>
  <div class="cont-card">
      <div class="card">
          <img src="../../assets/img/ruspa.jpg" alt="ruspa">
          <span class="titolo">Redeveloping Florida’s Remote Southern Coast</span>
          <span class="data">December 7th, 2015</span>
          <hr>
          <p class="desc">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>
      </div>
      <div class="card">
          <img src="../../assets/img/ponte.jpg" alt="ruspa">
          <span class="titolo">How We Manage Large Construction Projects</span>
          <span class="data">December 7th, 2015</span>
          <hr>
          <p class="desc">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>
      </div>
      <div class="card">
          <img src="../../assets/img/architettatura.jpg" alt="ruspa">
          <span class="titolo">Future proofing a modern home</span>
          <span class="data">December 6th, 2015</span>
          <hr>
          <p class="desc">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>
      </div>
  </div>
</template>

<script>
export default {
    name: 'CardNews',
}
</script>

<style lang="scss" scoped>
// Importazione variabili
@import "../../assets/style/variables.scss";

.cont-card{
    width: 62%;
    display: flex;
    justify-content: space-between;
    margin-top: 50px;
}

.card{
    width: 370px;
    background-color: $bianco;

    img{
        width: 370px;
    }

    span, p{
        display: block;
        padding: 0 20px;
    }

    .titolo{
        font-size: 25px;
        margin-top: 20px;
        margin-bottom: 5px;
        color: $scritta-nero;
    }

    .data{
        font-size: 13px;
        color: $scritta-grigio;
    }

    hr{
        margin: 0 auto;
        width: 330px;
        margin-top: 20px;
        margin-bottom: 20px;
        border: none;
        border-bottom: 1px solid $sfondo-grigio;
    }

    .desc{
        color: $scritta-grigio;
        line-height: 32px;
        padding-bottom: 20px;
    }
}
</style>