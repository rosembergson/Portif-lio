<template>
    <div>
        <slick ref="slick" :options="slickOptions">
                <slick
      ref="slick"
      :options="slickOptions">
      <a href="http://placehold.it/2000x1000"><img src="http://www.52dazhew.com/data/out/18/585489323-astronauts-in-space-wallpaper.png" alt=""></a>
      <a href="http://placehold.it/2000x1000"><img src="http://placehold.it/300x150" alt=""></a>
      <a href="http://placehold.it/2000x1000"><img src="http://placehold.it/300x150" alt=""></a>
      <a href="http://placehold.it/2000x1000"><img src="http://placehold.it/300x150" alt=""></a>
      <a href="http://placehold.it/2000x1000"><img src="http://placehold.it/300x150" alt=""></a>
    </slick>
        </slick>
    </div>

</template>




<script>
import Slick from 'vue-slick';

export default {
    components:{
        'slick': Slick
    },
    data() {
            return {
                slickOptions: {
                    infinite: true,
            slidesToShow: 3,
            slidesToScroll: 1,
            arrows: false,
            autoplay: true,
            infinite:true, 
            speed: 2000,
            autoplaySpeed: 3000,
    		responsive: 
    		[
            {
            breakpoint: 1120,
                settings: 
    			{	
                slidesToShow: 3,
                slidesToScroll: 1,
                }
            },
            {
                breakpoint: 800,
                settings: 
    			{
                slidesToShow: 2,
                slidesToScroll: 2
                }
            },
            {
                breakpoint: 600,
                settings: 
    	        {
                slidesToShow: 1,
                slidesToScroll: 1
                }
            }
    	    ]
                },
            };
        },

    mounted() {
        console.log(this.$options.name+' component successfully mounted');

        
    },
    methods:{
        next() {
                    this.$refs.slick.next()
            },
            prev() {
                    this.$refs.slick.prev()
            },
            reInit() {
                    // Helpful if you have to deal with v-for to update dynamic lists
                    this.$refs.slick.reSlick()
            }
    }
}
</script>

<style lang="scss">
    @import '../../scss/carousel.scss'
</style>