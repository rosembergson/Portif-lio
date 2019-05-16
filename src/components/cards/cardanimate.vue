<template>

    <div class="cardanimatebg" :class="{'active': isActive}" @mouseenter="showCard" >
        <img :src="cardanimate.img" alt="cardanimate.id">
        <div class="cardanimate_conteudo">
        <h4>{{cardanimate.name}}</h4>
        <p>{{cardanimate.text}}</p>
        <button type="button"> See more </button>
        </div>
    </div>

</template>

<script>
export default {
    data(){
        return{
            el: 'cardanimatebg',
            isActive: false
        }
    },
    props: {
        cardanimate: {
            type: Object,
            required: true
        }
    },
    methods: {
        showCard(){
            this.isActive = true;
        },
        hideCard(){
            this.isActive = false;
        }
    },
}

</script>

<style lang="scss">
    @import '../../scss/cardanimate.scss'
</style>