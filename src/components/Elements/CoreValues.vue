<template>
  <div class="cont-value">
      <div class="card">
          <i class="fas fa-home"></i>
          <span>Great Services</span>
          <hr>
          <p>Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia.</p>
      </div>
      <div class="card">
          <i class="far fa-sun"></i>
          <span>Highest Standards</span>
          <hr>
          <p>Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia.</p>
      </div>
      <div class="card">
          <i class="fas fa-users"></i>
          <span>Professional Team</span>
          <hr>
          <p>Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia.</p>
      </div>
      <div class="card">
          <i class="far fa-lightbulb"></i>
          <span>Creative Solutions</span>
          <hr>
          <p>Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia.</p>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Corevalues',
}
</script>

<style lang="scss" scoped>
// Importazione variabili
@import "../../assets/style/variables.scss";

.cont-value{
    width: 70%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 50px;
}

.fa-home{
    background-color: $sfondo-services;
    padding: 25px;
}

.fa-sun{
    background-color: $sfondo-standards;
    padding: 25px;
}

.fa-users{
    background-color: $sfondo-team;
    padding: 25px 20px;
}

.fa-lightbulb{
    background-color: $sfondo-solutions;
    padding: 25px 35px;
}

.card{
    width: 284px;
    text-align: center;
    position: relative;
    color: $scritta-grigio;

    i{
        font-size: 60px;
        color: $bianco;
        border-radius: 50%;

    }

    span{
        display: block;
        margin-top: 20px;
        margin-bottom: 20px;
    }

    hr{
        width: 20px;
        margin: 0 auto;
        margin-bottom: 20px;
    }

    p{
        line-height: 30px;
    }
}
</style>