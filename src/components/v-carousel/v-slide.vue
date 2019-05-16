<template>

    <slide>
        {{imagem.src}}
    </slide>

</template>

<script>
import { Carousel, Slide } from 'vue-carousel';
export default {
    props:{
        aux:{
            type:Object,
            required:true
        }
    },
    components:{
        Carousel,
        Slide,
    }
}
</script>

<style scoped>
    img{
        width:100px;
        height:100px;
    }
</style>