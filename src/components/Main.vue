<template>
    <main>
        <MainContent/>
    </main>
</template>

<script>
import MainContent from './section/MainContent.vue'

export default {
    name: 'Main',
    components :{
        MainContent,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/partial/variables.scss';
main{
    
    padding: 40px 0;
    color: $coloreQuarto;
    background: $coloreTerzo;
    
}

</style>