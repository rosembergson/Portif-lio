<template>
    <div class="headermenu_bg">
        <div class="headermenu_bg--div1">
            <img  class="headermenu_div1--img"style="width:100px; height:100px"src="../../assets/logo1.png" alt="logo_avengers" />
        </div>
        <div class="headermenu_bg--div2">
            <div class="div2--choosebuttonheader">
                <button type="button"> Sign in </button>
                <span> or </span>
                <button type="button"> Sign up </button>
            </div>
            <ul class="headermenu_div2--ul">
                <li v-for="menu in menus" :key="menu"> {{menu.name}} </li>
            </ul>
        </div>
    </div>
</template>

<script>
    import axios from 'axios'
    import config from '../../config/config.js'

export default {
    data(){
        return{
            menus: []
        }
    },
    created(){
        axios.get(`${config.apiURL}/headermenu`)
        .then((response)=>{
            this.menus = response.data
        })
    }
}
</script>

<style lang="scss">
    @import '../../scss/headermenu.scss'
</style>