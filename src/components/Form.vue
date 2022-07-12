<template>
<form>
    <div class="form-section">
        <input type="text" placeholder="關鍵字">
        <select name="商家區域">
            <option value="X">商家區域</option>
        </select>
        <select name="方案">
            <option value="X">方案</option>
        </select>
        <button class="search">搜尋</button>
    </div>
</form>
<div class="more-search">
    <img src="../assets/clean-search.png" alt="">
    <img class="more" src="../assets/More.png" alt="">
</div>
    

</template>

<script>
export default {

}
</script>

<style scoped>
form{ 
  margin-top: 10px;
  padding: 15px 10px 0 10px;
  background-color: rgba(255,244,198,0.2);
  display:flex;
  flex-direction: column;
  justify-content: center;
  align-items:center;

}
input{
  margin: 3px;
  border: none;
  width: 289px;
  height: 38px;
  padding: 0 10px;
  border: 1px solid #D8B93B;
  border-radius: 2rem;
  background-color: rgba(255,244,198,0.2);
}
select{
  margin: 1.5px;
  border: none;
  width: 289px;
  height: 38px;
  padding: 0 10px;
  border: none;
  border-radius: 2rem;
  background-color: #EFF0F4;
}
.search{
  margin: 3px;
  width: 187px;
  height: 38px;
  color: white;
  background-color: #2BABC6;
  border: none;
  border-radius: 2rem;
  padding: 10px 25px;

}
.more-search{
    display: flex;
    justify-content:right;
    align-items: center;
    padding-right: 300px;
    background-color: rgba(255,244,198,0.2);
    padding-bottom: 5px;
}
.more{
    display: none;
}
@media screen and (max-width: 1100px) {
.more{
    display:inline;
    margin: 0 10px;
}
select{
    display: none;
}
input{
    width:230px;
}
.search{
    width: 117px;
}
.form-section{
    display: flex;
}
}
@media screen and (max-width: 500px) {
.more-search{
    display: flex;
    justify-content:flex-end;
    align-items: center;
    padding-right: 10px;
    background-color: rgba(255,244,198,0);
}
}

</style>