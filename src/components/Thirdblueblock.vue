<template>
  <div  class="wroute">
    <div class="block2">
      <div class="second-block block">
        <div><p class="mainText">Организаторам</p>
          <p >Документы организаторам</p>
          <p >Услуги организаторам</p>
          <p >Рестораны и кафе</p>
          <p >Конгресс-центр</p>
          <p >Спорт-центр</p></div>

      </div>
      <div class="second-block block">
        <div><p class="mainText">Экспонентам</p>
          <p >Общие условия участия</p>
          <p >Услуги экспонентам</p>
          <p >Документы экспонентам</p>
          <p >Центр деловых контактов</p>
          <p >Забронировать гостиницу</p></div>
      </div>
      <div class="third-block block">
        <div>
          <p class="mainText">Посетителям</p>
          <p >Сервисы</p>
          <p >Онлайн-регистрация <br>на мероприятие </p>
          <p >Забронировать гостиницу</p>
          <p >Центр деловых контактов</p>
        </div>
      </div>
      <div class="forth-block block">
        <div>
          <p class="mainText">Прессе</p>
          <p>Аккредитация</p>
          <p>Пресс-служба</p>
          <p>Правила аккредитации</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TwoBlock",
  props:["TwoBlock"],
}
</script>
<style scoped>
*{
  color: white;
}
.mainText{
  margin-top: -175px;
  font-style: normal;
  font-weight: 500;
  font-size: 23px;
  line-height: 130%;
}
.inputStyle{
  width: 200px;
  height: 40px;
}
.wroute{
  display: flex;
  align-items: center;
  height: 391px;
  box-sizing: border-box;
  background: #2378FC;
  font-family: 'Circe';
  color: #FFFFFF;

}
.placeForInput{
  margin-top: 20px;
  display: flex;
}
.block{
  width: 220px;
}
.block > div{
  margin-bottom: 30px;
}
.block{
  width: 222px;
}
.block > div{
  margin-bottom: 0px;
}
.block2{
  width: 100%;
  display: flex;
  justify-content: center;
  gap: 90px;
}
.mainText{
  margin-top: -10px;
  justify-content: space-between;
  font-family: 'Plumb';
  font-size: 30px;
  padding-bottom: 30px;

}
p{
  padding-bottom: 10px;
}
</style>
