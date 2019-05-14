<template>
        <div class="cardlistanimatebg">
        <h1> Technology </h1>
            <cardanimate v-for="card in cards" :key="card" :cardanimate="card"/>
        </div>
</template>

<script>
    import axios from 'axios'
    import config from '../../config/config.js'
    import Cardanimate from './cardanimate.vue'
export default {
    components:{
        'cardanimate' : Cardanimate
    },
    data(){
        return{
            cards:[],
            el : '.cardlistanimatebg' 
        }
    },
    created(){
        axios.get(`${config.apiURL}/cardsanimation`)
        .then((response)=>{
            this.cards = response.data
        })
    }
}
</script>

<style lang="scss">
    @import '../../scss/cardanimate.scss'
</style>