<template>
        <div class="welcome" >
            
            <!-- <transition
            @before-enter="beforeEnter"
            @enter="enter"
            @after-enter="afterEnter"
            > -->
                <h2> Front-end Developer </h2>
                <p> I design and code beautifully simple things, and I love what I do. </p>
                <div class="welcomebg">
                    <img src="../../assets/17190358_1242978262484187_5264201441799392352_n.jpg" alt="avatar">
                </div>
            <!-- </transition> -->
            <div class="welcome_mouse">
                <span class="welcome_mouse--ball"></span>
            </div>
    </div>
</template>


<script>
export default {
    methods: {
        beforeEnter(el){
            el.style.opacity = 0;
        }
    },
}
</script>

<style lang="scss">
    @import '../../scss/welcome.scss'
</style>