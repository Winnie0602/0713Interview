<template>
  <div class="navBar">
    <!-- 手機版顯示 -->
    <a class="button-toggle" href="#">三</a>
    <img class="button-toggle" src="../assets/logo.png" alt="">
    <div class="button-toggle"></div>
    <!-- 寬螢幕時顯示 -->
    <div class="navBar-left">
      <img src="../assets/logo.png" alt="">
      <span><a href="#">我的商家</a></span>
      <span><a href="#">成效報表</a></span>
      <span><a href="#">基本資料</a></span>
      <span class="active"><a href="#">評價中心</a></span>
    </div>
    <div class="navBar-right">
      <img src="../assets/beauty.png" alt="">
      <a href="#">愛漂亮－林口</a>
      <button class="signOut">登出</button>
    </div>
  </div>
</template>

<script>
export default {
name: 'Navbar',

}
</script>


<style scoped>
.navBar{
  background-color: #29598F;
  height: 80px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  width: 100vw;
  
}
.navBar-right{
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.navBar-left{
  display: flex;
  justify-content: space-around;
  align-items: center;
}
a{
  margin:0 18px;
  padding: 10px 20px;
  text-decoration: none;
  color: white;
}
.navBar-left a:hover{
  background-color: rgba(255, 255, 255, 0.2);
  border-radius: 2rem;
}
/* RWD漢堡*/
.button-toggle {
  display: none;
}

.signOut{
  background-color: #29598F;
  border: 1px solid white;
  border-radius: 2rem;
  color: white;
  padding: 10px 25px;
}
@media screen and (max-width: 900px) {
.navBar{
  justify-content:space-between;
  padding: 0;
}
.button-toggle{
  display: inline-block;
  margin: 0;
  padding: 10px;
}
.navBar-left , .navBar-right{
  display: none;
}
}
</style>
