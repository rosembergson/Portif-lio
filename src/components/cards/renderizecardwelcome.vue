<template>
<div class="renderizecardwelcome_bg" style="background-image: url('https://downloadwallpaperhd.net/laptop-wallpapers/grand-theft-auto-v-4k-wallpaper-phone-For-Laptop-Wallpaper.jpg')">
    <headermenu/>
    <welcome/>
</div>
</template>

<script>
import Welcome from '../welcome/welcome.vue'
  import Headermenu from '../header/headermenu.vue'
export default {
    components:{
      'welcome' : Welcome,
      'headermenu' : Headermenu
    }
}
</script>


<style lang="scss">
    @import '../../scss/renderizecard.scss'
</style>
