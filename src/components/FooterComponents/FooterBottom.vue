<template>
    <div class="footer_bottom flex">
        <div>Copyrights 2017 <i class="far fa-copyright"></i> Mikado Themes</div>
        <div class="flex">
            <div>CALL +44 300 303 0266</div>
            <div class="social">
                <span>FOLLOW US</span>
                <a href="#" v-for="(elm, index) in socials" :key="index">
                    <i :class="elm"></i>
                </a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'FooterBottom',
    data() {
        return {
            socials : [
                'fab fa-twitter',
                'fab fa-instagram',
                'fab fa-facebook'
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .footer_bottom {
        height: 100px;
        line-height: 100px;
        border-top : 1px solid;
        justify-content: space-between;
        .social, .social i {
            margin-left: 20px;
            color: #b9b9b9;

        }

    }
</style>