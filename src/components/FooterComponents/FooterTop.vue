<template>
    <div class="footer_top">
        <FooterNavbar></FooterNavbar>
    </div>
</template>

<script>
import FooterNavbar from './FooterNavbar.vue'
export default {
    name : 'FooterTop',
    components : {
        FooterNavbar
    }
}
</script>

<style lang="scss" scoped>
    .footer_top {
        height: 400px;
        padding-top: 100px;
        background-color: grey;
    }
</style>