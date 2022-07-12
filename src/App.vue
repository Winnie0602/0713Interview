<template>
<Navbar />
<Store />
<Form />

<div class="handleChangeBtn">
    <div class="programming" @click="showRight = !showRight">執行中</div>
    <div class="apply" @click="showRight = !showRight">申請中</div>
</div>



<Filter />
<Left v-if="!showRight" />
<Right  v-if="showRight" />


  

</template>

<script>
import Navbar from './components/Navbar.vue'
import Store from './components/Store.vue'
import Form from './components/Form.vue'
import Filter from './components/Filter.vue'
import Left from './components/Left.vue'
import Right from './components/Right.vue'

import { ref } from 'vue' 

export default {
  name: 'App',
  components: {
    Navbar, Store, Form,Filter, Left, Right
  },
  setup(){
    const showRight = ref(false)

    return { showRight }
  }
}
</script>

<style>
*{
  box-sizing: border-box;
  padding:0;
  margin: 0;
}
h1, h2,h3,h4,h5{
  font-weight: normal;
}

a{
  margin:0 25px;
  text-decoration: none;
  color: white;
}

.handleChangeBtn{
  margin: 10px 18% ;
  display: flex;
  justify-content: flex-start;
  border-bottom: 1px solid #175993;
}
.programming , .apply{
  border-top: 1px solid #175993;
  border-left: 1px solid #175993;
  color:#175993;
  padding: 1rem;
}
.programming{
  border-bottom:1px solid white ;
}
.apply{
  border-top: 1px solid #C0C5D3;
  border-right: 1px solid #C0C5D3;
  color: #C0C5D3;
}
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
  .handleChangeBtn{
  margin: 10px 14% ;
}
}
@media screen and (max-width: 850px) {
  .handleChangeBtn{
  margin: 10px 10% ;
}
}



</style>
