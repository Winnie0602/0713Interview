<template>
    <div class="card">
        <div class="title">
            <div class="company">
                <img src="../assets/taipeiLogo.png" alt="">
                <div>
                    <h3>星和醫美台北店</h3>
                    <div class="yellow-btn">專業版</div>
                    <p>台北市重慶南路77號12樓</p>
                    <p>申請日期：2021.12.31</p>
                </div>
            </div>
            <button>選購方案</button>
            
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
    justify-content: space-between;
    align-items: center;
}
.company{
    display: flex;
    align-items: flex-start;
}
.company div{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    margin: 5px 0;
}


.yellow-btn{
    color: #D8B93B;
    border:1px solid #D8B93B;
    background-color: #FBF7E1;
    border-radius: 1rem;
    padding: 2px 5px ;
    margin: 0 5px;
}
button{
    color: white;
    border: 1px solid #46A77C;
    border-radius: 2rem;
    background-color: #46A77C;
    padding: 0.5rem 1.5rem;
}
h3{
    color: #185993;
}
p{
    color: #5A6268;
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
.title{
    display: flex;
    flex-direction: column;
    align-items:stretch;
    justify-content: center;
    margin: 1rem 0;
}
.title button{
    margin-top:1rem ;
}
}
</style>