<template>
    <div class="card">
        <div class="title">
            <img src="../assets/taipeiLogo.png" alt="">
            <div>
                <h3>星和醫美台北店</h3>
                <p>台北市重慶南路77號12樓</p>
            </div>
        </div>
        <div class="yellow">
            <div class="flex">
                <small class="yellow-btn">商家中心 專業版</small>
                <p>2020.12.31 - 2021.12.31</p>
            </div>
            <div class="percent">
                    <div>
                        <h2>2</h2>
                        <small>評論起始值</small>
                    </div>
                    <div>
                        <h2>200</h2>
                        <small>評論當前值</small>
                    </div>
                    <div>
                        <h2>198</h2>
                        <small>已增加評論數</small>
                    </div>
                    <div>
                        <h2>60%</h2>
                        <small>評論率</small>
                    </div>
                </div>
            <button>取得QRcode</button>
        </div>
        <div class="pink">
            <div class="flex">
                <small class="pink-btn">評價中心</small>
                <p>2020.12.31 - 2021.12.31</p>
            </div>
            <button>繼續申請</button>
        </div>
        
        
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.card{
    margin: 20px 18% ;
    border-bottom: 1px solid #C0C5D3;
    padding: 30px 0;
}
.title{
    display: flex;
}
.yellow , .pink{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.yellow button{
    color: #175993;
    border: 1px solid #175993;
    border-radius: 2rem;
    background-color: #fff;
    padding: 0.5rem 1.5rem;
}
.pink button{
    color: #D76c6c;
    border: 1px solid #D76c6c;
    border-radius: 2rem;
    background-color: #fff;
    padding: 0.5rem 1.5rem;
}
.flex{
    display: flex;
}
.flex small.yellow-btn{
    color: #D8B93B;
    border:1px solid #D8B93B;
    background-color: #FBF7E1;
    border-radius: 1rem;
    padding: 2px 5px ;
    margin: 0 5px;
}
.flex small.pink-btn{
    color: #D76C6C;
    border:1px solid #D76C6C;
    background-color: #FFE1E0;
    border-radius: 1rem;
    padding: 2px 5px ;
    margin: 0 5px;
}
.percent{
    display: flex;
}
.percent div{
    margin: 0 1rem;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.percent h2{
    color: #2babc6;
    font-weight: 700;
}
small{
    color: #D76c6c;
}
h3{
    color: #185993;
}
.percent small{
    color: #5a6268;
}
@media screen and (max-width: 1150px) {
.card{
    margin: 10px 14% ;
}
}
@media screen and (max-width: 850px) {
  .card{
  margin: 10px 10% ;
}
.yellow , .pink{
    display: flex;
    flex-direction: column;
    align-items:stretch;
    justify-content: center;
    margin: 1rem 0;
}
.yellow button,.pink button{
    margin: 15px 0;
}
}
</style>