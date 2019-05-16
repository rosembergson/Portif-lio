<template>
    <div class="cardlist">
        <h1></h1>
        <ul class="cardlist_bg">
            <card1 v-for="card in cards" :key="card" :card="card"/>
        </ul>
    </div>
</template>


<script>

    import axios from 'axios'
    import config from '../../config/config.js'
    import Card from './card.vue'

export default {
    data(){
        return{
            cards:[]
        }
    },
    methods:{

    },
    computed: {
        
    },
    created(){
        axios.get(`${config.apiURL}/card`)
        .then((response)=>{
            this.cards = response.data
        })
    },
    components:{
        'card1' : Card
    }
}
</script>

<style lang="scss">
    @import '../../scss/cardlist.scss'
</style>