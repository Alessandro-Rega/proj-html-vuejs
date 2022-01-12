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

      <CardSpecialist/>

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

      <section class="recent-work">
          <span>Explore Recent Work</span>
          <hr>
          <p>Lorem ipsum dolor sit amet. consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua ut enim ad minim veniam.</p>
          <CardCase/>
          <div class="all-projects">
            <span>view all projects</span>
          </div>
      </section>

      <section class="values">
          <span>Our Core Values</span>
          <hr>
          <p>Lorem ipsum dolor sit amet. consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua ut enim ad minim veniam.</p>
          <CoreValues/>
      </section>

      <section class="owners">
          <svg version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="padding:0;" fill="rgba(245,245,245,1)"><path d="M0 0 C55 180 100 0 100 0 Z"></path></svg>
          <span>Our Home Owners Say</span>
          <hr>
          <img src="../../assets/img/home-testimonial.jpg" alt="testimonial">
          <p>"No man but feels more of a man in the world if he have but a bit of ground that he can call his own. However small it is on the surface, it is four thousand miles deep; and that is a very handsome property."</p>
          <span>harry smith • new home owner</span>
          <div class="dot">
            <i class="fas fa-circle"></i>
            <i class="far fa-circle"></i>
          </div>
          <svg version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="padding:0;" fill="rgba(255,255,255,1)"><path d="M0 100 C40 0 60 0 100 100 Z"></path></svg>
      </section>
  </main>
</template>

<script>
import CardSpecialist from "../Elements/CardSpecialist.vue";
import CardCase from "../Elements/CardCase.vue";
import CoreValues from "../Elements/CoreValues.vue";

export default {
    name: 'Main',
    components:{
        CardSpecialist,
        CardCase,
        CoreValues,
    },
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

svg:last-child{
    transform: translateY(4px);
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

.recent-work{
    margin-top: 100px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-bottom: 50px;

    span{
        color: $scritta-nero;
        font-size: 35px;
    }

    hr:first-of-type{
        width: 10%;
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

    .all-projects{
        width: 80%;
        height: 50px;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        margin-top: 50px;

        span{
            text-transform: uppercase;
            font-size: 15px;
            color: $scritta-nero;
            cursor: pointer;
        }

        span:before{
            content: "";
            position: absolute;
            right: 150px;
            top: 23px;
            width: 400px;
            height: 10px;
            border-top: 2px solid #f5f5f5;
        }
        span:after{
            content: "";
            position: absolute;
            left: 150px;
            top: 23px;
            width: 400px;
            height: 10px;
            border-top: 2px solid #f5f5f5;
        }
    }
}

.values{
    margin-top: 100px;
    padding-top: 100px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding-bottom: 50px;
    background-color: #f5f5f5;

    span{
        color: $scritta-nero;
        font-size: 35px;
    }

    hr{
        width: 10%;
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

.owners{
    width: 100%;
    background-image: url("../../assets/img/home-parallax.jpg");
    background-position-y: -180px;
    text-align: center;
    background-color: #f5f5f5;

    span:first-of-type{
        display: block;
        color: $bianco;
        font-size: 35px;
        margin-top: 50px;
        margin-bottom: 30px;
    }

    hr{
        width: 12%;
        border: none;
        border-top: 2px solid $giallo;
        margin: auto;
        padding: 15px 0;
    }

    img{
        border-radius: 50%;
        margin-bottom: 20px;
    }

    p{
        width: 37%;
        margin: 0 auto;
        color: $bianco;
        font-size: 17px;
        font-weight: 600;
        line-height: 30px;
        font-style: italic;
    }

    span:last-of-type{
        display: block;
        color: $bianco;
        margin-top: 30px;
        text-transform: uppercase;
        font-size: 20px;
        font-weight: 600;
    }

    .dot{
        margin: 40px;
        color: $bianco;

        i{
            margin: 0 5px;
            font-size: 13px;
            cursor: pointer;
        }
    }
}
</style>