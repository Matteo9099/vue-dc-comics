<template>
   <footer>
        <FooterTop />
        <FooterBottom />
   </footer>
 
</template>


<script>
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

</style>