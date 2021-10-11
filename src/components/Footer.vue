<template>
    <footer>
        <div class="container">
            <FooterTop></FooterTop>
            <FooterBottom></FooterBottom>
        </div>
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
    footer {
        color: white;
        background-color: grey;
    }
</style>