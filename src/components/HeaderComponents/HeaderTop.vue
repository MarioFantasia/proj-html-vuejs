<template>
    <div class="header_top flex">
        <div class="logo col-2">
            <img src="../../assets/img/header/logo-light.png" alt="logo">
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
        /* per non applicare l'opacity all'elemento */
        position: relative;
        .logo {
            margin: auto 1px;
            img {
                width: 100%;
            }
        }
    }
</style>