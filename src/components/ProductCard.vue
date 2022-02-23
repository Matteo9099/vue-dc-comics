<template>
    <!-- Creo card con img e titolo -->
    <div class="card">
        <a href="#">
            <img class="card-thumb" :src="product.thumb" alt="">
            <p>{{ product.series }}</p>
        </a>
    </div>

</template>


<script>
    export default {
        name: 'ProductCard',
        props: ["product"],
    }
</script>


<style lang="scss" scoped>

    @import "../assets/style/variables.scss";

    .card{
        display: inline-block;
        width: calc(100% / 6 - 20px);
        margin: 25px 10px;
        transition: 0.3s;

        &:hover{
            box-shadow: 2px 2px 5px $secondaryColor;
            transform: scale(0.9);
        }

        a{
            color: #fff;
            text-decoration: none;

            .card-thumb {
                height: 200px;
                width: 200px;
                margin-bottom: 15px;
                object-fit: cover;
                width: 100%;
            }

            p{
                font-size: 0.8rem;
                text-transform: uppercase;
            }
        }
    }

</style>