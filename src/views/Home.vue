<template>
  <div class="home">
    <headermenu />
    <cardlist/>
    <!-- <foot/> -->
    <animatediv/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Headermenu from '../components/header/headermenu'
import Cardlist from '../components/cards/cardlist'
import Foot from '../components/footer/footer'
import Animatediv from '../components/animates/animatediv'
@Component({
  components: {
    'headermenu' : Headermenu,
    'cardlist' : Cardlist,
    'foot' : Foot,
    'animatediv' : Animatediv
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