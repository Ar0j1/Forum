<template>
  <div id="mainblock">
  <div id="main">
    <div id="text">
      <h2 class="head">Текущие и будущие мероприятия</h2>
      <p class="link"><a>Все мероприятия <img :src="Arrow"/></a></p>
    </div>
    <div id="elements">
      <div id="el">
        <img :src="item1"/>
        <p class="date">2 января 2020 г. – 7 января 2020 г.</p>
        <p id="red">ЭКСПО Ёлка</p>
        <p>Парк интерактивных развлечений</p>
      </div>
      <div id="el">
        <img :src="item2"/>
        <p class="date">5 февраля 2020 г. – 9 февраля 2020 г.</p>
        <p id="red">Junwex Петербург</p>
        <p>Выставка ювелирных изделий</p>
      </div>
      <div id="el">
        <img :src="item3"/>
        <p class="date">7 февраля 2020 г. – 9 февраля 2020 г.</p>
        <p id="red">Невский ларец</p>
        <p>Выставка-ярмарка народных художественных
          промыслов и ремесел</p>
      </div>
      <div id="el">
        <img :src="item4"/>
        <p class="date">14 февраля 2020 г. – 23 февраля 2020 г.</p>
        <p id="red">Понаехали!</p>
        <p>Специализированная арт-ярмарка</p>
      </div>
      <div id="el">
        <img :src="item5"/>
        <p class="date">18 февраля 2020 г. – 21 февраля 2020 г.</p>
        <p id="red">VET.CAMP</p>
        <p>Конференция для ветеринарных врачей</p>
      </div>
      <div id="el">
        <img :src="item6"/>
        <p class="date">26 февраля 2020 г. – 28 февраля 2020 г.</p>
        <p id="red">ExpoHoReCa</p>
        <p>Специализированная выставка</p>
      </div>


    </div>
  </div>
  </div>
</template>
<script>
export default {
  name: "BlockWithItems",
  props:["BlockComponents"],
  data(){
    return{
      item1: this.BlockComponents.allSrc.Item1,
      item2: this.BlockComponents.allSrc.Item2,
      item3: this.BlockComponents.allSrc.Item3,
      item4: this.BlockComponents.allSrc.Item4,
      item5: this.BlockComponents.allSrc.Item5,
      item6: this.BlockComponents.allSrc.Item6,
      Arrow: this.BlockComponents.allSrc.Arrow
    }
  }

}
</script>
<style>
#mainblock{
  background-color: #ffc41e;
  display: flex;
  align-items: center;
  width: 1920px;
  height: 984px;
}
img{
  width: 350px;
  height: 240px;

}
#text{

  display: grid;
  grid-template-columns: 1fr 1fr;

}
#main{
  width: 100%;
  display: grid;
  grid-template-columns: 1fr;
  justify-content: center;
  margin-left: 405px;
  margin-right: 405px;
  grid-row-gap: 55px;
  margin-top: 75px;
  /*padding-top: 50px;*/
}
#elements{
  /*margin-right: auto;*/
  /*margin-left: auto;*/
  display: grid;
  grid-template-columns: 350px 350px 350px;
  grid-column-gap: 30px;
  grid-row-gap: 40px;
  grid-auto-rows: 1fr 1fr 1fr;
}
#el{
  display: grid;
  grid-template-columns: 1fr ;
  grid-row-gap: 10px;
}
#red{
  color: red;
  font-size: 20px;
  font-weight: bold;
  height: 27px;
  font-family: 'Plumb';

}
div > p{
  height: 22px;
  font-family: 'Circe';
}
#text >h2{
  width: 474px;
  height: 39px;
  font-family: 'Plumb';
  font-style: normal;
  font-weight: 500;
  font-size: 30px;
  line-height: 130%;
}
.date{
  height: 19px;
}
.head{
  width: 474px;
  height: 39px;
}
.link{
  text-align: right;
  text-decoration-line: underline;
  color:black;

}
@font-face {
  font-family: 'Plumb';
  src: url("D:\@@@СКАЧКA@@@\Forum\forum\public\assets\Plumb.ttf");
}
@font-face {
  font-family: 'Circe';
  src: url("D:\@@@СКАЧКA@@@\Forum\forum\public\assets\circe.ttf");
}
a >img{
  width: 25px;
  height: 10px;
}
a:hover{
  color: black;
}
a:link{
  color: black;
}
a{
color:black;
}
</style>