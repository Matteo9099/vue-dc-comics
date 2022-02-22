<template>
    <div class="jumbotron"></div>
</template>

<script>
    export default {
    name: 'JumbotronComponents',

    }
</script>



<style lang="scss" scoped>

    @import "../assets/style/general.scss";

    .jumbotron{
        background: url('../assets/img/jumbotron.jpg') no-repeat;
        background-size: cover; 
        height: 350px;
        margin-top: 100px;
    } 

</style>
