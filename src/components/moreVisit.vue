<template>
    <div>
        <hr>
        <carousel :nav="false">
            <img src="https://placeimg.com/50/50/any?1">

            <img src="https://placeimg.com/50/50/any?2">

             <img src="https://placeimg.com/50/50/any?3">

             <img src="https://placeimg.com/50/50/any?4">
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