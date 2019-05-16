<template>
<div>
    <carousel >
    <slide>
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQhOVIIVQRlGi2CFDGSxOOUy8FdpRFxQqhsWDhnpzfSFARCRrQlmw"/>
    </slide>
    <slide>
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQhOVIIVQRlGi2CFDGSxOOUy8FdpRFxQqhsWDhnpzfSFARCRrQlmw"/>
    </slide>
    <slide>
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQhOVIIVQRlGi2CFDGSxOOUy8FdpRFxQqhsWDhnpzfSFARCRrQlmw"/>
    </slide>
    <slide>
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQhOVIIVQRlGi2CFDGSxOOUy8FdpRFxQqhsWDhnpzfSFARCRrQlmw"/>
    </slide>
    <slide>
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQhOVIIVQRlGi2CFDGSxOOUy8FdpRFxQqhsWDhnpzfSFARCRrQlmw"/>
    </slide>
    <slide>
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQhOVIIVQRlGi2CFDGSxOOUy8FdpRFxQqhsWDhnpzfSFARCRrQlmw"/>
    </slide>
    </carousel>
</div>
</template>




<script>
import { Carousel, Slide } from 'vue-carousel';
import Vslide from './v-slide'
export default {
    data(){
        return{
            images:[],
            data: [
          '<div class="example-slide">Slide 1</div>',
          '<div class="example-slide">Slide 2</div>',
          '<div class="example-slide">Slide 3</div>',
        ],
        }
    },
    components: {
        Carousel,
        Slide,
        'vslide' : Vslide
    },
    created(){
        axios.get(`${config.apiURL}/carousel`)
        .then((response)=>{
            this.images = response.data
        })
    },
}
</script>

<style lang="scss">
    
</style>