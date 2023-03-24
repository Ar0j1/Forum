<template>
     <div  class="block">
     <div class="boxb1">
        <p class="text1">Календарь <br>мероприятий</p>
        <p class="textp1">Подробнее</p> 
    </div>
     <div class="boxb2">    
        <p class="text1">Онлайн-заявка <br>на организацию<br>мероприятия</p>
        <p class="textp1">Подробнее</p>
    </div>   
    <div class="boxb3">
        <p class="text1">План <br>и инфраструктура<br> комплекса </p>
        <p class="textp1">Подробнее</p> 
    </div>
    <div class="boxb4">
        <p class="text1">Как добраться <br>до Экспофорума </p>
        <p class="textp1">Подробнее</p> 
    </div>
    </div>
</template>

<script> export default {
    name: "Block",
    props:["Block"],  
  }
</script>

<style>
    .block{
        box-sizing: border-box;
  width:255px;
  height:148px;
  font-family: 'Circe';
    line-height: 140%;
    }
.boxb1{
   background-color: #2378FC;
  margin:200px;
  position: absolute;
  display: grid;
  grid-template-columns: 1fr;
  width:255px;
  height:148px;
  left:505px;
  top:-199px;
}
.boxb2{
    background-color: #FFC41E;
  margin:200px;
  display: grid;
  grid-template-columns: 1fr;
  position: absolute;
  width:255px;
  height:180px;
  left:505px;
  top:-24px;
}
.boxb3{
    background-color: #F6404F;
  margin:200px;
  display: grid;
  grid-template-columns: 1fr;
  position: absolute;
  width:255px;
  height:180px;
  left:794px;
  top:-24px;
}
.boxb4{
   background-color: #30BCC9;
  margin:200px;
  position: absolute;
  width:255px;
  display: grid;
  grid-template-columns: 1fr;
  height:148px;
  left:794px;
  top:-199px;
}
.text1{
    font-style: normal;
    font-weight: 400;
    font-size:24px;
    line-height: 140%;
    margin-top:30px;
  height: 81px;
    margin-left:40px;
}
.textp1{
    margin-left:40px;
}
</style>