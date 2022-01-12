<template>
  <div class="hero">
      <h1>building inspiring spaces</h1>
      <p>We Build inspiring Residential & Commercial Spaces</p>
      <div>
        <button class="btn">explore recent work</button>
        <button class="btn">get a quote today</button>
      </div>

      <!-- Quadrati laterali -->
      <div class="quadrati">
        <div class="demos">
            <svg class="fss-after" width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M26 5.99994H6C5.44772 5.99994 5 6.44765 5 6.99994C5 7.55222 5.44772 7.99994 6 7.99994H26C26.5523 7.99994 27 7.55222 27 6.99994C27 6.44765 26.5523 5.99994 26 5.99994Z"></path>
            <path d="M24 2.99994H8C7.44772 2.99994 7 3.44765 7 3.99994C7 4.55222 7.44772 4.99994 8 4.99994H24C24.5523 4.99994 25 4.55222 25 3.99994C25 3.44765 24.5523 2.99994 24 2.99994Z"></path>
            <path fill-rule="evenodd" clip-rule="evenodd" d="M3 12.9999C3 10.7908 4.79086 8.99994 7 8.99994H25C27.2091 8.99994 29 10.7908 29 12.9999V24.9999C29 27.2091 27.2091 28.9999 25 28.9999H7C4.79086 28.9999 3 27.2091 3 24.9999V12.9999ZM11.2142 23.9962C11.0575 23.9962 10.9524 23.8414 11.0218 23.7026L15.8007 14.1131C15.8761 13.9623 16.0883 13.9623 16.1637 14.1131L16.5247 14.8371C18.9529 19.7192 15.6459 24.0041 11.2142 23.9962ZM18.3797 19.2906C18.4531 19.1399 18.6674 19.1399 18.7428 19.2906L20.9785 23.7065C21.0459 23.8414 20.9467 24.0001 20.796 24.0001H18.8578C17.4335 24.0001 16.6896 22.6194 17.2807 21.4371L18.3797 19.2906Z"></path>
            </svg>
            <span>Demos</span>
        </div>
        <div class="sale">
            <span>39</span>
            <span>On Sale</span>
        </div>
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
    position: relative;

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

    .quadrati{
        position: absolute;
        right: -2px;
        top: 20px;
    }

    .demos{
        background-color: #fff;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        padding: 10px;
        border-radius: 0.5em;
        margin-bottom: 10px;
        cursor: pointer;

        span{
            font-size: 12px;
            font-weight: bolder;
            color: #33475b;
        }

        svg{
            fill: #33475b;
        }
    }

    .sale{
        background-color: #fff;
        padding: 8px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border-radius: 0.5em;
        cursor: pointer;

        span:first-child{
            color: #65bc7b;
            font-weight: bold;
            font-size: 25px;
            position: relative;
            margin-left: 6px;

            &::before{
                content: "$";
                font-size: 15px;
                position: absolute;
                left: -10px;
            }
        }

        span:last-child{
            font-size: 12px;
            font-weight: bolder;
            color: #33475b;
        }
    }
}
</style>