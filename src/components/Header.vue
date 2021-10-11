<template>
    <header>
        <div class="container">
            <HeaderTop></HeaderTop>
            <HeaderBottom></HeaderBottom>
        </div>
    </header>
</template>

<script>
import HeaderTop from './HeaderComponents/HeaderTop.vue'
import HeaderBottom from './HeaderComponents/HeaderBottom.vue'
export default {
    name : 'Header',
    components : {
        HeaderTop,
        HeaderBottom
    }

}
</script>

<style lang="scss" scoped>
    header {
        background-image: url('../assets/img/header/course-9-f-img.jpg');
        background-size: cover;
        background-position: center;
        position: relative;
        /* aggiungere efetto filter */
        &::before { /* per applicare il filtro al bg */
            position: absolute;
            content: "";
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: black;
            opacity: 0.2;
        }
    }
</style>