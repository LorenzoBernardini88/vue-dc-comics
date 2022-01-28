<template>
    <div class="MainContent">
        <div class="jumbo"></div>
        <div class="comics_content">
            <div class="container">

            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MainContent',
        components:{
            
        }
    }
</script>

<style lang="scss" scoped>
@import '../../assets/style/partial/variables.scss';
    .jumbo{
        height: 300px;
        background-image: url('../../assets/img/jumbotron.jpg');
        background-position: contain;
        background-size: cover;
    }.comics_content{
        background: black ;
        height: 200px ;
        width: 100% ;
    }

    



</style>