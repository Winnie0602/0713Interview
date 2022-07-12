<template>
  <div class="store">
    <div class="store-left">
      <h3>我的商家</h3>
    </div>
    <div class="store-right">
      <img src="../assets/google.png" alt="">
      <img src="../assets/store-sign.png" alt="">
    </div>
  </div>
</template>

<script>
export default {
name: 'Navbar',

}
</script>


<style scoped>
.store{
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin-top: 20px;
}
.store img{
  margin: 0 20px;
}
div > h3{
  color: #5A6268;
}
@media screen and (max-width: 600px) {
  .store{
    flex-direction: column;
}
.store-left{
  border-bottom:1.5px solid #D8B93B;
  width: 90vw;
  text-align: center;
  margin-bottom: 10px;
  padding: 10px;
}
}
</style>
