<template>
  <div id="conteiner">
    <div id="ourblock">
      <p class="maintext">Организаторам</p>
      <p><a href="">Документы организаторам</a></p>
      <p><a href="">Услуги организаторам</a></p>
      <p><a href="">Выставочные площади</a></p>
      <p><a href="">Рестораны и кафе</a></p>
      <p><a href="">Конгресс-центр</a></p>
      <p><a href="">Спорт-центр</a></p>

    </div>
    <div id="ourblock">
      <p class="maintext">Экспонентам</p>
      <p><a href="">Общие условия участия</a></p>
      <p><a href="">Услуги экспонентам</a></p>
      <p><a href="">Документы экспонентам</a></p>
      <p><a href="">ентр деловых контактов</a></p>
      <p><a href="">Забронировать гостиницу</a></p>
      <p></p>
    </div>
    <div id="ourblock">
      <p class="maintext">Посетителям</p>
      <p><a href="">Сервисы</a></p>
      <p><a href="">Онлайн-регистрация на мероприятие</a></p>
      <p><a href="">Забронировать гостиницу</a></p>
      <p><a href="">Центр деловых контактов</a></p>
      <p></p>
      <p></p>
    </div>
    <div id="ourblock">
      <p class="maintext">Прессе</p>
      <p><a href="">Аккредитация</a></p>
      <p><a href="">ресс-служба</a></p>
      <p><a href="">Правила аккредитации</a></p>
      <p></p>
      <p></p>
      <p></p>
    </div>
  </div>
</template>
<style>
#conteiner{
  width: 1920px;
  height: 426px;
  display: grid;
  grid-template-columns: 210px 188px 188px 169px;
  grid-column-gap: 120px;
  background-color: #2378FC;
  color: white;
  padding-left: 400px;
  padding-right: 400px;
  padding-top: 75px;
}
#ourblock{

  display: grid;
  grid-template-columns: 1fr;
  /*grid-template-rows: 90px 22px 22px 22px 22px 22px 22px;*/
  grid-row-gap: 15px;
}
.maintext{
  font-size: 30px;
  height: 90px;
  font-family: Plumb;
}
p{
  height: 22px;
}
p>a{
  color: white;
  text-decoration: none;
  font-family: Circe;
}
a:hover{
  color: #FFC41E;
  text-decoration: underline;
  text-decoration-color: #FFC41E ;
}
@font-face {
  font-family: 'Plumb';
  src: url("../../public/assets/Plumb.ttf");
}
@font-face {
  font-family: 'Circe';
  src: url("../../public/assets/circe.ttf");
}
</style>