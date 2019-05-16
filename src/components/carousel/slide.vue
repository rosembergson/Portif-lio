<template>
    <div class="flip-box">
      <div class="flip-box-inner">
        <div class="flip-box-front">
            <img :src="slide.src" alt="slide">
        </div>
        
        <div class="flip-box-back">
                <div class="percentualbg">
                    <p>{{slide.porc}}</p>
                </div>
        </div>
  </div>
  </div>
</template>

<script>
export default {
    props:{
        slide:{
            type: Object,
            required: true
        }
    }
}
</script>

<style lang="scss">
    @import "../../scss/carousel.scss";
</style>