<template>
    <header>
        <img src="../../assets/img/construction_logo.png" alt="Logo Azienda">
        <div class="menu">
            <ul>
                <li v-for="voce in vociMenu" :key="voce">{{voce}}</li>
            </ul>
            <button class="btn">get quote</button>
        </div>
    </header>
</template>

<script>

export default {
  name: 'Header',
  components: {
  },
  props:{
      vociMenu: Array,
  }
}
</script>

<style lang="scss" scoped>
// Importazione variabili
@import "../../assets/style/variables.scss";

//stile
header{
    &::after{
        content: "";
        clear: both;
        display: table;
    }

    width: 100%;
    height: 130px;
    background-color: $bianco;

    img{
        margin-left: 100px;
        margin-top: 20px;
    }
}


.menu{
    float: right;
    margin-right: 60px;
    text-transform: uppercase;
    line-height: 130px;
    color: $scritta-nero;

    ul{
        margin-right: 20px;
        display: inline-block;

        li{
            font-size: 15px;
            display: inline-block;
            margin: 0 25px;
            cursor: pointer;
            position: relative;
        }

        li:first-child{
            color: $giallo;
        }

        & li:first-child::after{
            font-family: "Font Awesome 5 Free"; font-weight: 900; content: "\f0d7";
            position: absolute;
            color: $bianco;
            top: 66px;
            left: 12px;
            font-size: 40px;
        }
    }

    button{
        background-color: $giallo;
    }
}
</style>