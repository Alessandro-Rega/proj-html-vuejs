<template>
  <div class="cont-card">
      <div class="card">
          <img src="../../assets/img/ruspa.jpg" alt="ruspa">
          <span class="titolo">Redeveloping Florida’s Remote Southern Coast</span>
          <span class="data">December 7th, 2015</span>
          <hr>
          <p class="desc">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>

          <div class="card-hover">
              <div>
                <i class="fas fa-link"></i>
                <i class="fas fa-search"></i>
              </div>
              <span>Redeveloping Florida’s Remote Southern Coast</span>
              <span>Architecture, Buildings, Construction, News</span>
          </div>
      </div>
      <div class="card">
          <img src="../../assets/img/ponte.jpg" alt="ruspa">
          <span class="titolo">How We Manage Large Construction Projects</span>
          <span class="data">December 7th, 2015</span>
          <hr>
          <p class="desc">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>

          <div class="card-hover">
              <div>
                <i class="fas fa-link"></i>
                <i class="fas fa-search"></i>
              </div>
              <span>How We Manage Large Construction Projects</span>
              <span>Architecture, Buildings, Construction, News</span>
          </div>
      </div>
      <div class="card">
          <img src="../../assets/img/architettatura.jpg" alt="ruspa">
          <span class="titolo">Future Proofing A Modern Home</span>
          <span class="data">December 6th, 2015</span>
          <hr>
          <p class="desc">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>

          <div class="card-hover">
              <div>
                <i class="fas fa-link"></i>
                <i class="fas fa-search"></i>
              </div>
              <span>Future Proofing A Modern Home</span>
              <span>Architecture, Buildings, Construction, News</span>
          </div>
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
    position: relative;

    .card-hover{
        opacity: 0;
        width: 370px;
        height: 223px;
        background-color: $giallo;
        position: absolute;
        top: 0;
        left: 0;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        color: #fff;
        transition: 0.5s ease-in-out;

        &:hover{
            opacity: 1;
        }

        i{
            background-color: #fffaeb;
            padding: 15px;
            border-radius: 50%;
            font-size: 22px;
            color: #fed23f;
            margin: 10px 7px;
            cursor: pointer;
        }

        span{
            font-size: 18px;
            margin-bottom: 10px;
            text-align: center;
        }

        span:last-child{
            font-size: 12px;
        }
    }

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