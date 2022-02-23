<template>
    <div id="footer-bottom">
        <!-- Containeer footer bottom -->
        <div class="container d-flex d-center d-justify-between">
            <!-- Parte sx container con pulsante -->
            <div id="sign-up"><a href="#">SIGN-UP NOW!</a></div>
            <!-- Parte dx container con social -->
            <div id="social">
                <h3>FOLLOW US</h3>
                <!-- Lista Social -->
                <ul>
                    <li>
                        <a href="#">
                            <img src="../../assets/img/footer-facebook.png" alt="Logo Facebook">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../../assets/img/footer-twitter.png" alt="Logo twitter">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../../assets/img/footer-youtube.png" alt="Logo youtube">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../../assets/img/footer-pinterest.png" alt="Logo pinterest">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../../assets/img/footer-periscope.png" alt="Logo periscope">
                        </a>
                    </li>

                </ul>
            </div>
        </div>
    </div>
</template>


<script>
    export default {
        name: 'FooterBottom',
    }
</script>


<style lang="scss" scoped>
    // Importo regole
    @import "../../assets/style/general.scss";
    @import "../../assets/style/utils.scss";
    @import "../../assets/style/variables.scss";


    .container{
        padding: 20px 0;
    }

    #footer-bottom{
        background-color: #303030;

        #sign-up{
            a{
                color: #fff;
                padding: 15px;
                text-decoration: none;
                border: 2px solid $secondaryColor;

                &:hover{
                    background-color: $secondaryColor;
                }
            }
        }
    }

    #social{
        display: flex;
        align-items: center;

        h3{
            color: $secondaryColor;
            margin-right: 5px;
        }

        ul{
            display: inline-block;
            list-style-type: none;
            display: flex;
        }

        li{
            margin: 0 10px;
        }

    }

</style>