<template>
  <div class="home">
    <headermenu />

    <welcome/>

    <cardlistanimation/>
    <animatediv/>
    <cardlist/>
  <div class="app">
  </div>
  <carousel/>
    <particules/>
    <pictureanimation/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Headermenu from '../components/header/headermenu'
import Cardlist from '../components/cards/cardlist'
import Foot from '../components/footer/footer'
import Animatediv from '../components/animates/animatediv'
import Particules from '../components/animates/particulesanimation'
import Welcome from '../components/welcome/welcome'
import Carousel from '../components/carousel/carousel'
import Pictureanimation from '../components/animates/picturesanimation'
import CardlistAnimation from '../components/cards/cardlistanimate'
@Component({
  components: {
    'headermenu' : Headermenu,
    'cardlist' : Cardlist,
    'foot' : Foot,
    'animatediv' : Animatediv,
    'particules' : Particules,
    'welcome' : Welcome,
    'carousel' : Carousel,
    'pictureanimation' : Pictureanimation,
    'cardlistanimation' : CardlistAnimation
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