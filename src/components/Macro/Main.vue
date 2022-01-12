<template>
  <main>
      <section class="help">
          <span>Do You Have A Construction Project We Can Help With?</span>
          <button class="btn">get a free quote</button>
      </section>

      <section class="specialist">
          <span>Specialists In Modern Construction</span>
          <hr>
          <p>Lorem ipsum dolor sit amet. consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua ut enim ad minim veniam.</p>
      </section>

      <CardSpecialist v-bind:cardList="cardList"/>

      <section class="stats">
          <svg version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="padding:0;" fill="rgba(255,255,255,1)"><path d="M0 0 C55 180 100 0 100 0 Z"></path></svg>
          <div class="cont-icon">
            <div class="icon">
                <i class="fas fa-suitcase"></i>
                <span class="numero">3534</span>
                <span>planning applications</span>
            </div>
            <div class="icon">
                <i class="far fa-building"></i>
                <span class="numero">896</span>
                <span>completed projects</span>
            </div>
            <div class="icon">
                <i class="fas fa-users"></i>
                <span class="numero">172</span>
                <span>trained professionals</span>
            </div>
            <div class="icon">
                <i class="fas fa-globe"></i>
                <span class="numero">19</span>
                <span>international offices</span>
            </div>
          </div>
          <svg version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="padding:0;" fill="rgba(255,255,255,1)"><path d="M0 100 C40 0 60 0 100 100 Z"></path></svg>
      </section>
  </main>
</template>

<script>
import CardSpecialist from "../Elements/CardSpecialist.vue";

export default {
    name: 'Main',
    components:{
        CardSpecialist,
    },
    data(){
        return{
            cardList: [
                {
                    nome: 'Buildings',
                    immagine: 'far fa-building',
                    testo: 'Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.'
                },
                {
                    nome: 'Renovate',
                    immagine: 'fas fa-sync',
                    testo: 'Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.'
                },
                {
                    nome: 'Construct',
                    immagine: 'fas fa-home',
                    testo: 'Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.'
                },
                {
                    nome: 'Exclusive',
                    immagine: 'fas fa-truck',
                    testo: 'Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
// Importazione variabili
@import "../../assets/style/variables.scss";

.help{
    width: 100%;
    height: 150px;
    background-color: $giallo;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: relative;

    span{
        font-size: 35px;
        color: $scritta-nero;
    }

    button{
        background-color: $nero;
        color: $bianco;
        position: absolute;
        bottom: -20px;
        border: 2px solid white;
        padding: 12px 50px;
        font-size: 15px;
    }
}

.specialist{
    margin-top: 150px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-bottom: 50px;

    span{
        color: $scritta-nero;
        font-size: 35px;
    }

    hr{
        width: 15%;
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

.stats{
    width: 100%;
    background-image: url("../../assets/img/home.jpg");
    background-position-y: -300px;
}

.cont-icon{
    width: max-content;
    margin: 0 auto;
    margin-top: 120px;
    margin-bottom: 120px;
}

.icon{
    display: inline-block;
    text-align: center;
    margin: 0 50px;

    i{
        color: $giallo;
        font-size: 80px;
        margin-bottom: 10px;
    }

    .numero{
        display: block;
        font-size: 50px;
        color: $giallo;
    }

    span:last-child{
        color: $bianco;
        font-size: 14px;
        font-weight: bold;
        text-transform: uppercase;
    }
}
</style>