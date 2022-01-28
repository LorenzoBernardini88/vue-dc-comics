<template>
    <div class="MainContent">
        <div class="jumbo">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MainContent',
    }
</script>

<style lang="scss" scoped>
@import '../../assets/style/partial/variables.scss';
.MainContent{
    height: 300px;
    .jumbo{
        height: 100%;
        background-image: url('../../assets/img/jumbotron.jpg');
        background-position: contain;
        background-size: cover;
    }
    
}

</style>