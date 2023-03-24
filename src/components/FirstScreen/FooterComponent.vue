<template>
<div  class="wrapper">
  <div class="footer">
    <div class="first-block block">
      <div>
        <p class="mainText">О компании</p>
        <p>О нашей компании</p>
        <p>Вакансии</p>
        <p>Партнеры</p>
        <p>Контакты</p>
      </div>
      <div>
        <p class="mainText">Организаторам</p>
        <p>Преимущества площадки</p>
        <p>Структура комплекса</p>
        <p>Онлайн-заявка на организацию</p>
        <p>Документы организаторам</p>
      </div>
    </div>
    <div class="second-block block">
      <div><p class="mainText">Экспонентам</p>
        <p>Общие условия участия</p>
        <p>Услуги экспонентам</p>
        <p>Документы экспонентам</p>
        <p>Забронировать гостиницу</p></div>
      <div>
        <p class="mainText">Посетителям</p>
        <p>Сервисы</p>
        <p>Онлайн-регистрация</p>
        <p>Забронировать гостиницу</p>
        <p>Центр деловых контактов</p>
      </div>
    </div>
    <div class="third-block block">
      <div>
        <p class="mainText">Прессе</p>
        <p>Аккредитация</p>
        <p>Пресс-служба</p>
        <p>Правила аккредитации</p>
      </div>
      <div>
        <p class="mainText">Приложение</p>
        <img :src="apple"/>
        <img :src="google"/>
      </div>
    </div>
    <div class="forth-block block">
      <div>
        <p class="mainText">Мы в соц. сетях</p>
        <img :src="contct"/>

      </div>
      <div>
        <p class="mainText">Подписка на новости</p>
        <p>Получайте все самые последние новости о мероприятиях в Экспофоруме.</p>
        <div class="placeForInput">
          <div><input type="text" class="inputStyle"/></div>
          <img :src="messImg"/>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: "FooterComponent",
  props:["ForFooterComponent"],
  data(){
    return{
      contct: this.ForFooterComponent.allSrc.contact,
      messImg: this.ForFooterComponent.allSrc.messageImg,
      apple: this.ForFooterComponent.allSrc.apple,
      google: this.ForFooterComponent.allSrc.google
    }
  }

}
</script>

<style scoped>
*{
  color: white;
}
.inputStyle{
  width: 200px;
  height: 40px;
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
 .mainText{
 
   font-style: normal;
   font-weight: 500;
   font-size: 21px;
   line-height: 130%;
 }
 .wrapper{
   display: flex;
   align-items: center;
   height: 390px;
   width: 1920px;
   background-color: LightSeaGreen;
 }
 .footer{

   width: 100%;
   display: flex;
   justify-content: center;
   gap: 100px;
 }
</style>