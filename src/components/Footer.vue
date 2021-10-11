<template>
    <footer>
        <FooterTop></FooterTop>
        <FooterBottom></FooterBottom>
    </footer>
</template>

<script>
import FooterTop from './FooterComponents/FooterTop.vue'
import FooterBottom from './FooterComponents/FooterBottom.vue'
export default {
    name : 'Footer',
    components : {
        FooterTop,
        FooterBottom
    }
}
</script>

<style lang="scss" scoped>

</style>