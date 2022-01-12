<template>
  <section>
      <div class="card">
        <div class="img">
            <i class="far fa-building"></i>
        </div>
        <h3>Buildings</h3>
        <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>
      </div>
      <div class="card">
        <div class="img">
            <i class="fas fa-sync"></i>
        </div>
        <h3>Renovate</h3>
        <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>
      </div>
      <div class="card">
        <div class="img">
            <i class="fas fa-home"></i>
        </div>
        <h3>Construct</h3>
        <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>
      </div>
      <div class="card">
        <div class="img">
            <i class="fas fa-truck"></i>
        </div>
        <h3>Exclusive</h3>
        <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>
      </div>
  </section>
</template>

<script>
export default {
    name: 'CardSpecialist',
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