<template>
    
    <!-- Creo header con logo e menù -->
    <header>
        <div class="container">
            <a href="#"><img src="../assets/img/dc-logo.png" alt="DC logo"></a>
           
            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index">
                        <a href="#" :class="{current: link.current}">{{link.text}}</a>
                    </li>
                </ul>
            </nav>
        </div> 

    </header>

</template>


<script>
    export default {
        name: "HeaderComponents",
        data() {
            return {
                links: [
                    { text: "CHARACTERS", url: "#", current: false },
                    { text: "COMICS", url: "#", current: true },
                    { text: "MOVIES", url: "#", current: false },
                    { text: "TV", url: "#", current: false },
                    { text: "GAMES", url: "#", current: false },
                    { text: "COLLECTIBLES", url: "#", current: false },
                    { text: "VIDEOS", url: "#", current: false },
                    { text: "FANS", url: "#", current: false },
                    { text: "NEWS", url: "#", current: false },
                    { text: "SHOP", url: "#", current: false },
                ]
            }
        }
    }
</script>


<style lang="scss" scoped>

    @import "../assets/style/general.scss";
    @import "../assets/style/variables.scss";

    header{
        position: fixed;
        top: 0;
        left: 0;
        background-color: #fff;
        height: 100px;
        width: 100%;

        img{
            width: 70px;
            height: 70px;
            object-fit: cover;
        }

        ul{
            display: flex;

            li{ 
                margin: 0 10px;
                list-style-type: none;
            }

            a{
                text-decoration: none;
                padding: 40px 0;
                color: $primaryColor;

                &.current{
                    color: $secondaryColor;
                    border-bottom: 5px solid $secondaryColor;
                }

                &:hover{
                    color: $secondaryColor;
                    border-bottom: 5px solid $secondaryColor;
                }
            }
        }
    }

    .container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        height: 100%;
    }

</style>