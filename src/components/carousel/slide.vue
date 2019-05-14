<template>
    <div class="slide">
        <img :src="slide.src" alt="image"/>
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

<style scoped>
    img{
        max-width:100%;
    }
    .slide{
        display: inline-block;
    }
</style>