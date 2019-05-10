<template>
  <div class="home">
    <headermenu />
    <cardlist/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Headermenu from '../components/header/headermenu'
import Cardlist from '../components/cards/cardlist'
@Component({
  components: {
    'headermenu' : Headermenu,
    'cardlist' : Cardlist
  }
})
export default class Home extends Vue {}
</script>


<style scoped>
  .home{
    width:100%;
    height:100%;
  }
</style>