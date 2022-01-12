<template>
  <div class="cont-case">
      <div class="casa">
          <img src="../../assets/img/casa1.jpg" alt="casa">

          <div class="casa-hover">
              <div>
                <i class="fas fa-link"></i>
                <i class="fas fa-search"></i>
              </div>
              <span>Florida Health Facility</span>
              <span>Commercial</span>
          </div>
      </div>
      <div class="casa">
          <img src="../../assets/img/casa2.jpg" alt="casa">

          <div class="casa-hover">
              <div>
                <i class="fas fa-link"></i>
                <i class="fas fa-search"></i>
              </div>
              <span>Florida Health Facility</span>
              <span>Commercial</span>
          </div>
      </div>
      <div class="casa">
          <img src="../../assets/img/casa3.jpg" alt="casa">

          <div class="casa-hover">
              <div>
                <i class="fas fa-link"></i>
                <i class="fas fa-search"></i>
              </div>
              <span>Florida Health Facility</span>
              <span>Commercial</span>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'CardCase',
    props:{
        caseList: Array,
    }
}
</script>

<style lang="scss" scoped>
.cont-case{
    margin: 0 auto;
    margin-top: 40px;
}

.casa{
    display: inline-block;
    margin: 0 17px;
    position: relative;

    img{
        width: 380px;
    }

    .casa-hover{
        opacity: 0;
        width: 380px;
        height: 380px;
        background-color: #fed23f;
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
        }

        span:last-child{
            font-size: 15px;
        }
    }
}
</style>