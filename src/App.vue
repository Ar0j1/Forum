<template>
  <UpperBoxes ></UpperBoxes>
  <Thirdblueblock></Thirdblueblock>

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
import UpperBoxes from './components/UpperBoxes.vue';
import Thirdblueblock from './components/Thirdblueblock.vue';

export default{
  name:"App",
  components: {
    UpperBoxes,
    Thirdblueblock,
    BlockWithItems,
    FooterComponent
  },
  data() {
    return {

      ForFooterComponent: {
        allSrc:{
          vk:require('../public/assets/footer/vk.svg'),
          fb:require('../public/assets/footer/fb.svg'),
          yt:require('../public/assets/footer/yt.svg'),
          inst:require('../public/assets/footer/inst.svg'),
          contact:require('../public/assets/FrameContact.svg'),
          messageImg:require('../public/assets/footer/Group 2.svg'),
          apple: require('../public/assets/footer/1Frame.svg'),
          google:require('../public/assets/footer/Frame.svg')
        }
      },
      BlockComponents: {
        allSrc:{
          Item1:require("../public/assets/Eventsimg/event1.svg"),
          Item2:require("../public/assets/Eventsimg/event2.svg"),
          Item3:require("../public/assets/Eventsimg/event3.svg"),
          Item4:require("../public/assets/Eventsimg/event4.svg"),
          Item5:require("../public/assets/Eventsimg/event5.svg"),
          Item6:require("../public/assets/Eventsimg/event6.svg"),
          Arrow:require("../public/assets/arrow.svg"),


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


