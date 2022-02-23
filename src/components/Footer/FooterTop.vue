<template>
    
    <section id="footer_top">
        <div class="container">
            <!-- Creo delle sezioni con lista dei link-->
            <nav>
                <section v-for="(footer_nav, index) in footer_navs" :key="index">
                    <!-- titolo dinamico -->
                    <h3>{{ footer_nav.title }}</h3>
                    <!-- link dinamici -->
                    <ul>
                        <li v-for="(text, index) in footer_nav.texts" :key="index">
                            <a href="#">{{ text }}</a>
                        </li>
                    </ul>
                </section>
            </nav>
            <div class="logo_dc_bg"></div>
        </div>
    </section>

</template>


<script>
    export default {
        name: 'FooterTop',        
        data() {
            return{
                footer_navs: [
                    // link nav 1
                    {
                        title: "DC COMICS",
                        texts: [
                            'Characters',
                            'Comics',
                            'Movies',
                            'TV',
                            'Games',
                            'Videos',
                            'News'
                        ],
                    },
                     // link nav 2
                    {
                        title: "SHOP",
                        texts: ['Shop DC', 'Shop DC Collectibles']
                    },
                     // link nav 3
                    {
                        title: "DC",
                        texts: [
                            'Terme Of Use',
                            'Privacy policy(New)',
                            'Ad Choices',
                            'Advertisting',
                            'Jobs',
                            'Subscriptions',
                            'Talent Workshops',
                            'CPSC Certificates',
                            'Ratings',
                            'Shop Help',
                            'Contact Us'
                        ],
                    },
                     // link nav 4
                     {
                         title: "SITES",
                         texts: [
                             'DC',
                             'MAD Magazine',
                             'DC kids',
                             'DC Universe',
                             'DC Power Visa'
                         ]
                     }

                ]
            }
        }
    }
</script>


<style lang="scss" scoped>
    // importo regole
    @import "../../assets/style/general.scss";

    #footer_top{
        background: url('../../assets/img/footer-bg.jpg') no-repeat;
        background-size: cover;

        nav{
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            margin: 25px 0;
            padding-right: 100px;

            section {
                margin: 0 20px;

                h3{
                    margin: 15px 0;
                    color: #fff;
                }

                ul{
                    display: inline-block;
                    list-style-type: none;

                    li{
                        padding: 3px 0;

                        a{
                            text-decoration: none;
                            font-size: 0.8rem;
                            color: rgb(189, 184, 184);

                            &:hover{
                                text-decoration: underline;
                            }
                        }
                    }
                }
            }
        }

        .container{
            display: flex;
            justify-content: space-between;
            max-height: 400px;
        }

        .logo_dc_bg{
            background: url('../../assets/img/dc-logo-bg.png') no-repeat;
            background-size: cover;
            width: 500px;
        }
    }

</style>