<template>
  
    <nav>
        <div class="container">
            <ul>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        <span>DIGITAL COMICS</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        <span>DC MERCHANDISE</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        <span>SUBSCRIPTION</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        <span>COMIC SHOP LOCATOR</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        <span>DC POWER VISA</span>
                    </a>
                </li>
            </ul>
        </div>
    </nav>

</template>



<script>
    export default {
        name: 'MainNavMenu',
    }
</script>



<style lang="scss" scoped>

    @import "../assets/style/variables.scss";

    nav {
        background-color: $secondaryColor;
        // padding: 30px 0;
        color: #fff;

        ul{
            display: flex;
            justify-content: space-around;
            list-style-type: none;

            li{
                display: flex;
                align-items: center;

                &:hover{
                    background-color: rgb(53, 172, 241);
                }

                a{
                    display: flex;
                    align-items: center;
                    text-decoration: none;
                    color: #fff;
                    padding: 30px 5px;


                    img{
                        height: 50px;
                        margin-right: 10px;
                    }

                    span{
                        font-size: 0.8rem;
                    }
                }
            }
        }
    }

</style>