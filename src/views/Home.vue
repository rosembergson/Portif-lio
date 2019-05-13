<template>
  <div class="home">
    <headermenu />

    <welcome/>

    <animatediv/>
    <cardlist/>
    <carousel/>
    
    <particules/>


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
@Component({
  components: {
    'headermenu' : Headermenu,
    'cardlist' : Cardlist,
    'foot' : Foot,
    'animatediv' : Animatediv,
    'particules' : Particules,
    'welcome' : Welcome,
    'carousel' : Carousel
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
  
</style>