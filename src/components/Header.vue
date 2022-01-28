<template>
  <header>
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="">
      <ul>
        <li v-for="(elemento,indice) in links" :key='indice'><a :class="{active: elemento.current}" href="#">{{elemento.text}}</a></li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return{
      links:[
        {
          text: "Carachters",
          url: "#",
          current: true,
        },
        {
          text: "Comics",
          url: "#",
          current: false,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/partial/variables.scss';

header{
  padding: 10px 0;

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  img{
    width: 80px;
    height: 80px;
  }
  ul{
      display:flex;
      gap: 20px;
      font-size: 18px;

      li{
      list-style-type:none;
      
          a{
            padding: 35px 0;
            color: $coloreTerzo;
            text-decoration: none;

            &:hover{
              color: $colorePrimo;
            }
            &.active{
              border-bottom: solid 4px $colorePrimo;
            }
          }
      }
    }
}

</style>
