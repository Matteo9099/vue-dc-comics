<template>
  
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

    .card{
        display: inline-block;
        width: calc(100% / 6 - 20px);
        margin: 25px 10px;

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