<template>
  <div id="Moremainbox">

  <div id="Mainmanu">
    <a class="logo">
      <img src="..\..\public\assets\logotip.png"/>
    </a>
    <div class="gap1">
    <div id="Menutext">
      <p style="width: auto">О комплексе</p>
      <p style="width: auto">О компании</p>
      <p style="width: auto">Новости</p>
      <p style="width: auto">Медиа-банк</p>
      <p style="width: auto">Контакты</p>
    </div>
      <div class="gap2">
    <a class="sort">
      <img src="..\..\public\assets\Search.png"/>
    </a>
        <div class="gap3">
    <a class="globus">
      <img src="..\..\public\assets\Globe.png"/>
    </a>
    <p>English</p>
        </div>
      </div>
    </div>
  </div>
<hr>
    <div id="secondbox">

      <div id="owntext">
        <p class="text1">ЭКСПОФОРУМ </p>
        <p class="text2">конгрессно-выставочный центр <br>Санкт-Петербурга</p>
        <p class="text3"><a>Подробнее<img src="..\..\public\assets\arrow.svg"/></a></p>
      </div>
      <div id="ownblock">
        <div id="block1" style="background-color: #2378FC;"><p style="font: bold; font-size: 22px; line-height:25px">Календарь<br>мероприятий</p>
          <p ><a style="color: white">Подробнее<img src="..\..\public\assets\arrow.svg"/></a></p></div>
        <div id="block1" style="background-color: #30BCC9;"><p style="font: bold; font-size: 22px; line-height:25px">Как добраться<br>до Экспофорума</p>
          <p ><a style="color: white">Подробнее<img src="..\..\public\assets\arrow.svg"/></a></p></div>
        <div id="block1" style="background-color: #FFC41E;"><p style="font: bold; font-size: 22px; line-height:25px">Онлайн-заявка<br>на организацию<br>мероприятия</p>
          <p ><a style="color: white">Подробнее<img src="..\..\public\assets\arrow.svg"/></a></p></div>
        <div id="block1" style="background-color: #F6404F;"><p style="font: bold; font-size: 22px; line-height:25px">План<br>и инфраструктура <br>комплекса</p>
          <p ><a style="color: white">Подробнее<img src="..\..\public\assets\arrow.svg"/></a></p></div>
      </div>
    </div>
</div>
</template>

<script>

</script>

<style>
#Moremainbox{
  display: grid;
  grid-template-columns: 1920px;
  grid-template-rows: 90px 2px 708px;
  background-image: url("../../public/assets/bgc.png");
  height: 800px;
  width: 1920px;
}
#Mainmanu{
display: grid;
  grid-template-columns: 175px  1fr;
  grid-column-gap:311px ;
  margin-top: 30px;
  margin-left: 180px;
  margin-right: 180px;
  height: 60px;
  color: white;

}
hr {
  border: none; /* Убираем границу */
  background-color: white; /* Цвет линии */
  color: white; /* Цвет линии для IE6-7 */
  height: 2px; /* Толщина линии */
}
.gap1{
  display: grid;
  grid-template-columns: 586px  152px;
  grid-column-gap:315px ;
}
.gap2{
  display: grid;
  grid-template-columns: 20px 100px;
  grid-column-gap:70px ;
}
.gap3{
  display: grid;
  grid-template-columns: 20px  1fr;
  grid-column-gap:11px ;
}
#Menutext{
  display: grid;
  grid-template-columns: auto auto auto auto auto;
  text-align: center;
  grid-column-gap: 47px;
}
.logo{
  width: 175px;
  height: 24px;
}
.logo > img{
  width: 175px;
  height: 24px;
}
.sort > img{
  width: 20px;
  height: 18px;
}
.globus> img{
  width: 20px;
  height: 18px;
}
#secondbox{
  margin-left:180px;
  margin-right:180px;
  display: grid;
  grid-template-columns: 1fr 1fr;
  color: white;
  margin-top: 184px;
}
#owntext{
  margin-left: 30%;
  display: grid;
  grid-template-columns: 1fr;
  grid-row-gap: 34px;
  grid-template-rows: 74px 68px 22px;
}
#ownblock{
  display: grid;
  grid-template-columns: 255px 255px;
  grid-template-rows: 148px 175px;
  grid-gap: 30px;
  margin-top: 15%;
}
.text1{
  font-size: 64px;
  margin-top: 0px;
  margin-left: 0px;
  font-family: Plumb;

}
.text2{
  font-size: 24px;
  font-family: Circe;

}
.text3{
  font-family: Circe;

}
.text3> a{
  color: white;
}
.text3 > img{
  width: 20px;
  height: 22px;

}
#block1{
  display: grid;
  grid-template-columns: 1fr;
  padding-top: 30px;
  padding-left: 40px;
  grid-row-gap: 30px;

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