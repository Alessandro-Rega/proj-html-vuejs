<template>
  <footer>

    <div class="footer-top">
    <div class="left">
      <img src="../../assets/img/footer-logo.png" alt="Logo">
      <p>We are specialists in the construction of unique and exclusive properties. Our work inspires. We pride ourselves on delivering outstanding quality and design for leading clients across the world.</p>
      <button class="btn">learn more</button>
    </div>

    <div class="center-left">
      <h3>latest tweets</h3>
      <div class="logo">
        <img src="../../assets/img/logo-twitter.png" alt="logo">
      </div>
        <div class="tweet">
          <span>ThemeFusion</span>
          <span>@Theme_Fusion</span>
          <img src="../../assets/img/tweet.svg" alt="tweet">
          <p>Do you need sublime WordPress hosting for your next website? Take advantage of exclusive partner offers that we have secured just for you; & launch your site in seconds with <a href="">#avada</a> on WP Engine hosting & get 30% Off this Black Friday <a href="">bit.ly/3kjLLE2#BlackFriday2020</a></p>
          <img src="../../assets/img/tweet-foto.png" alt="post">
        </div>
    </div>

    <div class="center-right">
      <h3>Contact us today</h3>
      <ul>
        <li v-for="(item, i) in contatti" :key="i">
          <i :class="item.icona"></i>
          <div>
            {{item.testo}}
          </div>
        </li>
      </ul>
    </div>

    <div class="right">
      <h3>find us</h3>
      <img src="../../assets/img/map.png" alt="mappa">
    </div>
    </div>

    <div class="footer-bottom">
      <span>copyrigth 2012 - 2015 avada theme by <span>theme fusion</span>  |  all rights reserved  |  powered by <span>wordpress</span></span>
      <div>
        <i class="fab fa-facebook-f"></i>
        <i class="fab fa-twitter"></i>
        <i class="fab fa-youtube"></i>
        <i class="fab fa-instagram"></i>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer',
    props:{
      contatti: Array,
    },
}
</script>

<style lang="scss" scoped>
// Importazione variabili
@import "../../assets/style/variables.scss";

footer{
  width: 100%;
  height: 650px;
  background-color: $nero;

  .footer-top{
    display: flex;
    background-color: $nero;
    padding: 100px 80px;
  }

  .footer-bottom{
    width: 100%;
    height: 80px;
    background-color: #111111;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-left: 110px;

    span{
      text-transform: uppercase;
      color: $scritta-grigio;
      font-size: 11px;

      span{
        color: #a0a0a0;
      }
    }

    div{
      color: $scritta-grigio;
      margin-right: 80px;

      i{
        margin: 0 10px;
        cursor: pointer;
      }
    }
  }

  h3{
    text-transform: uppercase;
    color: $giallo;
  }
}

.left{
  width: 25%;
  margin-left: 30px;

  p{
    width: 95%;
    color: #a0a0a0;
    line-height: 35px;
    margin: 20px 0;
  }

  button{
    background-color: $giallo;
    padding: 10px 25px;
    font-size: 15px;

    &:hover{
      background-color: $bianco;
    }
  }
}

.center-left{
  width: 25%;
  margin-right: 50px;

  &::after{
    content: "";
    clear: both;
    display: table;
  }

  h3{
    margin-bottom: 40px;
  }

  .logo{
    float: left;
    margin-left: 10px;

    img{
      width: 35px;
      border-radius: 50%;
      margin-right: 10px;
    }
  }

  .tweet{
    width: 80%;
    display: inline-block;
    position: relative;

    span:first-child{
      display: block;
      color: $bianco;
      font-size: 15px;
      font-weight: 600;
    }

    span:last-of-type{
      color: #c2cbd2;
      font-size: 14px;
    }

    img[alt="tweet"]{
      width: 20px;
      position: absolute;
      top: 5px;
      right: -20px;
    }

    p{
      width: 107%;
      font-size: 13px;
      color: $bianco;
      margin-bottom: 30px;
      margin-top: 10px;
    }

    a{
      text-decoration: none;
      color: #2b7bb9;
    }

    img[alt="post"]{
      width: 350px;
    }
  }
}

.center-right{
  width: 25%;

  ul{
    list-style: none;
    margin-top: 40px;

    li{
      color: #a0a0a0;
      margin: 10px 0;

      i{
        float: left;
        margin-top: 3px;
      }

      div{
        width: 60%;
        display: inline-block;
        font-size: 14px;
        margin-left: 10px;
      }
    }
  }
}

.right{
  width: 25%;

  img{
    width: 330px;
    margin-top: 40px;
  }
}
</style>