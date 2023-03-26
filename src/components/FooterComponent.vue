<template>
  <div class="wrapper">
    <div class="footer">
      <div class="first-block block">
        <div>
          <p class="mainText">О компании</p>
          <p><a href="">О нашей компании</a></p>
          <p><a href="">Вакансии</a></p>
          <p><a href="">Партнеры</a></p>
          <p><a href="">Контакты</a></p>
        </div>
        <div>
          <p class="mainText">Организаторам</p>
          <p><a href="">Преимущества площадки</a></p>
          <p><a href="">Структура комплекса</a></p>
          <p><a href="">Онлайн-заявка на организацию</a></p>
          <p><a href="">Документы организаторам</a></p>
        </div>
      </div>
      <div class="second-block block">
        <div><p class="mainText">Экспонентам</p>
          <p><a href="">Общие условия участия</a></p>
          <p><a href="">Услуги экспонентам</a></p>
          <p><a href="">Документы экспонентам</a></p>
          <p><a href="">Забронировать гостиницу</a></p></div>
        <div>
          <p class="mainText">Посетителям</p>
          <p><a href="">Сервисы</a></p>
          <p><a href="">Онлайн-регистрация</a></p>
          <p><a href="">Забронировать гостиницу</a></p>
          <p><a href="">Центр деловых контактов</a></p>
        </div>
      </div>
      <div class="third-block block">
        <div>
          <p class="mainText">Прессе</p>
          <p><a href="">Аккредитация</a></p>
          <p><a href="">Пресс-служба</a></p>
          <p><a href="">Правила аккредитации</a> </p>
        </div>
        <div>
          <p class="mainText">Приложение</p>
          <img :src="apple"/>
          <img :src="google"/>
        </div>
      </div>
      <div class="forth-block block">
        <div class="contact">
          <p class="mainText">Мы в соц. сетях</p>
          <a href=""><img :src="yt" style=" width:35px"/></a>
          <a href=""><img :src="vk" style="width:44px"/></a>
          <a href=""><img :src="fb" style="width:13.52px;height: 25px;"/></a>
          <a href=""><img :src="inst" style="width:25px"/></a>

        </div>
        <div>
          <p class="mainText">Подписка на новости</p>
          <p>Получайте все самые последние новости о мероприятиях в Экспофоруме.</p>
          <div class="placeForInput">
            <div><input type="text" class="inputStyle" placeholder="Введите ваш e-mail" /></div>
            <a  href=""><img :src="messImg"/></a>
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
      vk: this.ForFooterComponent.allSrc.vk,
      fb: this.ForFooterComponent.allSrc.fb,
      yt: this.ForFooterComponent.allSrc.yt,
      inst: this.ForFooterComponent.allSrc.inst,
      messImg:this.ForFooterComponent.allSrc.messageImg ,
      apple:this.ForFooterComponent.allSrc.apple ,
      google:this.ForFooterComponent.allSrc.google
    }
  }

}
</script>

<style scoped>
*{
  color: white;
}
@font-face {
  font-family: 'Plumb';
  src: url("../../public/assets/Plumb.ttf");
}
@font-face {
  font-family: 'Circe';
  src: url("../../public/assets/circe.ttf");
}

.contact>a{

  margin-right: 25px;
  height: 25px;
}

.inputStyle{
  width: 215px;
  height: 40px;
  border-width: 1;
  padding: 0 0 0 0 ;
}
::placeholder {
  color: #999; /* изменить цвет текста на серый */
  font-family: 'Circe';
  text-indent: 20px;
}

.placeForInput{
  margin-top: 20px;
  display: flex;
  width: 215px;
  height: 40px;

}
.block{
  width: 220px;

}
.block > div{
  margin-bottom: 30px;
}
p{
  font-family: 'Circe';
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 135%;
  margin-bottom: 10px;
}
.mainText{
  font-family: 'Plumb';
  margin-bottom: 15px;
  font-style: normal;
  font-weight: 500;
  font-size: 21px;
  line-height: 130%;
}
.wrapper{
  display: flex;
  align-items: center;
  height: 476px ;
  width: 100%;
  background-color: LightSeaGreen;
}
.footer{
  margin-bottom:110px ;
  width: 100%;
  display: flex;
  justify-content: center;
  gap: 100px;
}
a{
  text-decoration: none;
}
a:hover {
  color: #FFC41E; /* Цвет ссылки при наведении */
  text-decoration: underline; /* Добавляем подчёркивание */
}
</style>