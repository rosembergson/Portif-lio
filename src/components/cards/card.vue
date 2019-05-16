<template>
    <li class="card_bg">
        <div class="card_bg--img">
            <img :src="card.src" :alt="card.id">
        </div>
        <div class="card_bg_conteud">
            <div class="card_conteud--text1">   
                <h5> {{card.titule5}} </h5>
                <p>  {{card.conteud2}} </p>
            </div>
        </div>
        <div class="card_conteud--text3">
            <button type="button"> Inscrever </button>
        </div>
    </li>
</template>

<script>
export default {
    props:{
        card:{
            type: Object,
            required:true
        }
    }
}
</script>

<style lang="scss">
    @import '../../scss/card.scss'
</style>