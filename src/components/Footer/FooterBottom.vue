<template>
    <div id="footer-bottom">
        <div class="container d-flex d-center d-justify-between">
            <div id="sign-up"><a href="#">SIGN-UP NOW!</a></div>
            <div id="social">
                <h3>FOLLOW US</h3>
                <ul>
                    <li class="debug"></li>
                    <li class="debug"></li>
                    <li class="debug"></li>
                    <li class="debug"></li>
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
            }
        }
    }

    #social{
        display: flex;
        align-items: center;

        h3{
            color: $secondaryColor;
        }

        ul{
            display: inline-block;
            list-style-type: none;
            display: flex;
        }

        li{
            margin: 0 10px;
        }

        .debug{
            height: 30px;
            width: 30px;
            border-radius: 50%;
            background-color: blue;
        }
    }

</style>