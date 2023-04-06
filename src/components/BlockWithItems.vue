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
        <ItemOfForm
            v-for="Item of ArrayItems" :key='Item.id'
            v-bind:ItemOfForm = 'Item'
        >

        </ItemOfForm>

      </div>
      <div id="knopka"><button id="createnewform" @click="showForm = !showForm">Add new Form</button></div>
      <form v-if="showForm" @submit.prevent>
        <input @input="title = $event.target.value" v-bind:value="title"  type="text" placeholder="Заголовок услуги">
        <input @input="description = $event.target.value" v-bind:value="description" type="text" placeholder="Описание услуги">
        <input @input="date = $event.target.value" v-bind:value="date" type="text" placeholder="Описание услуги">
        <label>
          <input  type="file" @input="image = $event.target.value" v-bind:value="image" >
          <span>Выберите фото</span>
        </label>
        <button @click="createPost">Добавить услугу</button>
      </form>
    </div>
  </div>
</template>
<script>
import ItemOfForm from './ItemOfForm.vue'

export default {
  name: "BlockWithItems",
  props: ["BlockComponents"],
  data() {
    return {
      item1: this.BlockComponents.allSrc.Item1,
      item2: this.BlockComponents.allSrc.Item2,
      item3: this.BlockComponents.allSrc.Item3,
      item4: this.BlockComponents.allSrc.Item4,
      item5: this.BlockComponents.allSrc.Item5,
      item6: this.BlockComponents.allSrc.Item6,
      Arrow: this.BlockComponents.allSrc.Arrow,
      ArrayItems: [],
      title: "",
      description: "",
      date: "",
      image: [],
      showForm: false,
    };
  },
  methods: {
    createPost() {
      console.log(this.image.split("\\").slice(-1));
      this.image = require(`../../public/assets/${this.image.split("\\").slice(-1)}`);
      const newPost = {
        id: Date.now(),
        title: this.title,
        description: this.description,
        image: this.image,
        date: this.date
      };
      this.ArrayItems.push(newPost);
      this.title = "";
      this.image = [];
      this.description = "";
      this.date = "";
    }
  },
  components: { ItemOfForm }
}
</script>
<style>
#knopka{
  display: grid;
  grid-template-columns: 150px;
  justify-content: center;
}
form{
  display: grid;
  grid-template-columns: 150px;
  justify-content: center;
}
#mainblock{
  background-color: #ffc41e;
  display: flex;
  align-items: center;
  width: auto;
  padding-bottom: 70px;
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
  src: url("../../public/assets/Plumb.ttf");
}
@font-face {
  font-family: 'Circe';
  src: url("../../public/assets/circe.ttf");
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
.link> a{
  color:black;
}
</style>