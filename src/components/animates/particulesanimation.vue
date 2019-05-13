<template>
    <div class="particulesanimationbg">
            <vue-particles
            color="#dedede"
            :particleOpacity="0.7"
            :particlesNumber="80"
            shapeType="circle"
            :particleSize="4"
            linesColor="#dedede"
            :linesWidth="1"
            :lineLinked="true"
            :lineOpacity="0.4"
            :linesDistance="150"
            :moveSpeed="3"
            :hoverEffect="true"
            hoverMode="grab"
            :clickEffect="true"
            clickMode="push"
            >
        </vue-particles>
        <div class="particulesanimation_contact" >
            <contact/>
        </div>
    </div>
</template>

<script>

import Contact from '../footer/contact.vue'

export default {
    components:{
        'contact' : Contact
    }
}
</script>

<style scoped>

.particulesanimationbg{
    width:100%;
    top:0;
    left:0;
    margin:0;
     /* background:#ff4a5a; */
    position:relative;
    background-image: url('https://s2.best-wallpaper.net/wallpaper/3840x2160/1902/Astronaut-planet-stars-beautiful-space_3840x2160.jpg');
    background-position: center;
                background-size: cover;
                background-repeat: no-repeat;
                object-fit: cover;
}


</style>