<template>
  <div class="cont">
    <a class="logo">
        <img src="../../../public/assets/logotip.png"/>
        </a>
        <a class="sort">
        <img src="../../../public/assets/Search.png"/>
        </a>
        <a class="globus">
        <img src="../../../public/assets/Globe.png"/>
        </a>
        <h3 class="English">English</h3>
    <FirstScreenMenu class="menu" v-bind:MenuItems = 'MenuItems'></FirstScreenMenu>
   
    <div class="form">
      <p class="text1">ЭКСПОФОРУМ </p>
      <p class="text2">конгрессно-выставочный центр <br>Санкт-Петербурга</p>
      <Block></Block>
      <p class="text3">О комплексе </p>
    </div>
  </div>
</template>
<script>
import FirstScreenMenu from "@/components/FirstScreen/FirstScreenMenu.vue";
import Block from "@/components/FirstScreen/Block.vue";
export default {
  name: "FirstScreen",
  components:{
    FirstScreenMenu,
    Block
  },
  data(){
    return{
      MenuItems:[
        {id:1, title: "О комплексе"},
        {id:2, title: "О компании"},
        {id:3, title: "Новости"},
        {id:4, title: "Медиа-банк"},
        {id:5, title: "Контакты"}
      ]
    }
}}
</script>

<style scoped>

.logo{
  float:left;
   margin-top:36px; 
   margin-left:110px;
}
.pod{
position: absolute;
width: 72px;
height: 19px;
left:910px;
top: 439px;
font-family: 'Circe';
font-style: normal;
font-weight: 400;
font-size: 14px;
line-height: 135%;
}
.English{
  position: absolute;
width: 51px;
height: 22px;
left: 1495px;
top: 42px;
font-family: 'Circe';
font-style: normal;
font-weight: 400;
font-size: 16px;
line-height: 135%;
text-align: right;
}
.sort{
  float:right;
   margin-top:41px; 
   margin-right:300px;
}

.globus{
  float:right;
   margin-top:41px; 
   margin-right:-104px;
}
*{
  margin: 0;
  padding: 0;
  color: white;
  font-size: 16px;
}
.form{
  display: flex;
  flex-direction: column;
  position: absolute;
  width: 533px;
  height: 68px;
  left: 100px;
  top: 383px;
}
.text3{
font-family: 'Circe';
font-style: normal;
font-weight: 400;
font-size: 16px;
  line-height: 40px;
  text-align: center;
  margin-top: 103px;
  margin-left: 40px;
}
.text2{
  font-family: 'Circe';
  position: absolute;
width: 533px;
height: 68px;
left: 105px;
top: -35px;
font-family: 'Circe';
font-style: normal;
font-weight: 400;
font-size: 24px;
line-height: 140%;
margin-top: 40px;
  margin-left: 134px;
}
.text1{
  font-family: 'Plumb';
  font-style: normal;
  font-weight: 680;
  font-size: 49px;
  line-height: 120%;
  text-transform: uppercase;
  color: #FFFFFF;
  left: 105px;
  top: 20px;
  margin-left: 236px;
  margin-top:-70px;
}
.cont{
  background-image: url('../../../public/assets/bgc.png');
  height: auto;
  height: 800px;
  object-fit: contain;
  width: 100%;
 
}
.menu{
  position: absolute;
  height: 100px;
  align-items: center;
  width: 100%;
  border-bottom:1px solid #FFFFFF;
  justify-content: center;
  position: absolute;
}


</style>
