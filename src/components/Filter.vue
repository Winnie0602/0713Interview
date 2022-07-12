<template>
  <div class="filter">
    <p>共 10 筆商家</p>
    <div class="img">
      <img src="../assets/6.png" alt="">
      <img src="../assets/5.png" alt="">
      <img src="../assets/4.png" alt="">
      <img class="none" src="../assets/9.png" alt="">
      <img class="none" src="../assets/1.png" alt="">
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.filter{
  margin: 10px 18% ;
  display: flex;
  justify-content: space-between;
}
.img{
  display: flex;
}
.img img{
  padding: 0 3px;
}
@media screen and (max-width: 1150px) {
.filter{
    margin: 10px 14% ;
}
}
@media screen and (max-width: 850px) {
  .filter{
  margin: 10px 10% ;
}
  .filter p{
    display: none;
  }
  .none{
    display: none;
  }
  
}

</style>