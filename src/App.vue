<template>
 <FirstScreen></FirstScreen>
<TwoBlock></TwoBlock>
 <div id='app'>
    <BlockWithItems :BlockComponents="BlockComponents"/>
    <FooterComponent :ForFooterComponent="ForFooterComponent"/>

  </div>
</template>
<script>
import TwoBlock from './components/TwoBlock.vue';
import FooterComponent from './components/FooterComponent.vue';
import FirstScreen from './components/FirstScreen/FirstScreen.vue';
import BlockWithItems from './components/BlockWithItems.vue';
export default{
  name:"App",
  components: {
    TwoBlock,

    FirstScreen,
    BlockWithItems,
    FooterComponent
  },
data() {
    return {

      ForFooterComponent: {
        allSrc:{
          contact:require('../public/assets/FrameContact.svg'),
          messageImg:require('../public/assets/footer/Group 2.svg'),
          apple: require('../public/assets/footer/1Frame.svg'),
          google:require('../public/assets/footer/Frame.svg')
        }
      },
      BlockComponents: {
        allSrc:{
          Item1:"./src/components/img/img_1.svg",
          Item3:"./src/components/img/img_2.svg",
          Item4:"./src/components/img/img_3.svg",
          Item5:"./src/components/img/img_4.svg",
          Item6:"./src/components/img/img_5.svg",
          Item2:"./src/components/img/img.svg",
          Arrow:"./src/components/img/arrow.svg",


        }
      }
    }
  }
}
</script>
<style>
*{
  margin:0; 
}

</style>


