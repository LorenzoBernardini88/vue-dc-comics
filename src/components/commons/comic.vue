<template>
    <div class="comicContainer">
        <div class="cover">
            <img :src="elemento.thumb" >
        </div>
        <span>{{elemento.series}}</span>
    </div>
</template>

<script>



export default {
    name: 'comic',
    props:{
        elemento : Object,
    }
}
</script>

<style lang="scss" scoped>
    .comicContainer{
            width: 160px;
            text-align: left;
            img{
                width: 100%;
                height: 160px;
                object-position: top;
                object-fit:cover;
            }
        }
            


</style>