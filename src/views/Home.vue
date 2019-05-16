<template>
  <div class="home">
    <hoopercarousel/>

    <cardlistanimation/>

    <particules/>

    <carousel/>

    <cardlist/>

    <foot/>

  </div>
</template>

<script >
import { Component, Vue } from "vue-property-decorator"
import Cardlist from "../components/cards/cardlist"
import Foot from "../components/footer/footer"
import Animatediv from "../components/animates/animatediv"
import Particules from "../components/animates/particulesanimation"
import Carousel from "../components/carousel/carousel"
import CardlistAnimation from "../components/cards/cardlistanimate"
import hoopercarousel from "../components/v-carousel/hoopercarousel"
@Component({
  components: {
    
    'cardlist' : Cardlist,
    'foot' : Foot,
    'animatediv' : Animatediv,
    'particules' : Particules,
    'carousel' : Carousel,
    
    'cardlistanimation' : CardlistAnimation,
    'hoopercarousel' : hoopercarousel
  }
})
export default class Home extends Vue {}
</script>


<style scoped>
  .home{
    width:100%;
    height:100%;
  }
  animatediv{
    width:100vw;
  }
  .app{
    max-width:900px;
  }
</style>