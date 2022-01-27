<template>
    <footer>
        <div class="top_footer">
            <div class="container">
                <div class="content_top" v-for="(elemento,indice) in links" :key="indice">
                    <img :src="elemento.img" alt="">
                    <span>{{elemento.text}}</span>
                </div>
            </div>
        </div>
        <div class="middle_footer">
            <div class="container">
                <div class="content_middle">
                    <div class="list">
                        <div class="list_title">dc comics</div>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                    </div>
                    <div class="list">
                        <div class="list_title">dc</div>
                        <ul>
                            <li><a href="#">Terms Of use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="list">
                        <div class="list_title">sites</div>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                    <div class="list">
                        <div class="list_title">shop</div>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>



<script>
export default {
    name: 'Footer',
    data() {
    return{
        links:[
                {
                text: "DIGITAL COMICS",
                img:require("../assets/img/buy-comics-digital-comics.png"),
                current: false,
                },
                {
                text: "DC MERCHANDISE",
                img: require("../assets/img/buy-comics-merchandise.png"),
                current: false,
                },
                {
                text: "COMIC SHOP LOCATOR",
                img: require("../assets/img/buy-comics-subscriptions.png"),
                current: false,
                },
                {
                text: "SUBSCRIPTIONS",
                img: require("../assets/img/buy-comics-shop-locator.png"),
                current: false,
                },
                {
                text: "DC POWER VISA",
                img: require("../assets/img/buy-dc-power-visa.svg"),
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
    footer{
        
        .top_footer{
            padding: 20px 0;
            color: $coloreQuarto;
            background: $colorePrimo;

            .container{
                display: flex;
                align-items: center;
                justify-content: space-around;

                .content_top{
                    width: 15%;
                    font-size: 12px;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    gap: 5px;
                    
                    img{
                        width: 20%;
                    }
                }
            }
        }
        .middle_footer{
            padding: 25px 0;
            background-image: url('../assets/img/footer-bg.jpg');
            background-repeat: no-repeat;

            .content_middle{
                width: 35%;
                display: flex;
                flex-wrap: wrap;
                gap: 40px;
                .list .list_title{
                    color: $coloreQuarto;
                    font-size: 16px;
                    font-weight: bold;
                    text-transform: uppercase;
                    margin-bottom:8px ;

                }
                .list ul li {
                    list-style-type:none;
                    line-height: 20px;
                    a{
                        color:#797979;
                        font-size: 12px;
                        text-decoration: none;
                        
                    }
                }
            }   
        }
    }

</style>