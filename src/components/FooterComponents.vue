<template>
   <footer>
        <FooterTop />
        <FooterBottom />
   </footer>
 
</template>


<script>
    // importo FooterTop e FooterBottom nel Footer principale
    import FooterTop from './Footer/FooterTop.vue';
    import FooterBottom from './Footer/FooterBottom.vue';
    
    export default {
        name: 'FooterComponents',
        components: {
            FooterTop,
            FooterBottom
        }
    }
</script>


<style lang="scss" scoped>

    @import "../assets/style/general.scss";

</style>