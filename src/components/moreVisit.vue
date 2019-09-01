<template>
    <div>
        <hr>
        <carousel :nav="false">
            <img src="https://placeimg.com/300/300/tech">

            <img src="https://placeimg.com/300/300/tech">

             <img src="https://placeimg.com/300/300/tech">

             <img src="https://placeimg.com/300/300/tech">
        </carousel>
    </div>
</template>

<script>
import carousel from 'vue-owl-carousel'

export default {
    name:'moreVisit',
    components:{
        carousel
    }
}
</script>

<style  scoped>
img{
    padding:1%;
    border-radius: 5px;
}
</style>