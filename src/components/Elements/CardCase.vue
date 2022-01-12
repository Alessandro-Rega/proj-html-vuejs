<template>
  <div class="cont-case">
      <div class="casa">
          <img src="../../assets/img/casa1.jpg" alt="casa">
      </div>
      <div class="casa">
          <img src="../../assets/img/casa2.jpg" alt="casa">
      </div>
      <div class="casa">
          <img src="../../assets/img/casa3.jpg" alt="casa">
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
    img{
        width: 380px;
    }
}
</style>