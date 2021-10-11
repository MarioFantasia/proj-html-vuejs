<template>
    <div class="header_top flex">
        <div class="logo">
            <img src="../../assets/img/header/logo-light.png" alt="">
        </div>
        <HeaderNavbar></HeaderNavbar>
    </div>
</template>

<script>
import HeaderNavbar from './HeaderNavbar.vue'
export default {
    name : 'HeaderTop',
    components : {
        HeaderNavbar
    }
}
</script>

<style lang="scss" scoped>
    .header_top {
        height: 80px;
        justify-content: space-between;
        background-color:red;
        .logo {
            width: 200px;
            margin: auto 1px;
            img {
                width: 100%;
            }
        }
    }
</style>