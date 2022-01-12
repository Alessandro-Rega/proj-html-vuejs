<template>
  <section>
      <div class="card">
        <div class="img">
            <i class="far fa-building"></i>
        </div>
        <h3>Buildings</h3>
        <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>

        <div class="card-hover">
            <span>artfully crafted</span>
            <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>
            <button class="btn">get a quote</button>
        </div>
      </div>
      <div class="card">
        <div class="img">
            <i class="fas fa-sync"></i>
        </div>
        <h3>Renovate</h3>
        <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>

        <div class="card-hover">
            <span>artfully crafted</span>
            <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>
            <button class="btn">get a quote</button>
        </div>
      </div>
      <div class="card">
        <div class="img">
            <i class="fas fa-home"></i>
        </div>
        <h3>Construct</h3>
        <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>

        <div class="card-hover">
            <span>artfully crafted</span>
            <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>
            <button class="btn">get a quote</button>
        </div>
      </div>
      <div class="card">
        <div class="img">
            <i class="fas fa-truck"></i>
        </div>
        <h3>Exclusive</h3>
        <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>

        <div class="card-hover">
            <span>artfully crafted</span>
            <p>Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.</p>
            <button class="btn">get a quote</button>
        </div>
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
    position: relative;
}

.card-hover{
    opacity: 0;
    width: 400px;
    height: 284px;
    background-color: $giallo;
    position: absolute;
    top: 0;
    left: 0;
    transition: 0.2s ease-in-out;
    text-align: center;
    border-radius: 0.7em;
    padding: 30px 0 0 0;

    &:hover
    {
        opacity: 1;
    }

    span{
        display: block;
        text-transform: uppercase;
        margin-bottom: 20px;
    }

    p{
        line-height: 35px;
    }

    button{
        padding: 12px 30px;
        background-color: #ffe07b;

        &:hover{
            background-color: $nero;
            color: $bianco;
        }
    }
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