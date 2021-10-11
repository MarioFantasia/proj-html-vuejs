<template>
    <header>
        <HeaderTop></HeaderTop>
        <HeaderBottom></HeaderBottom>
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

</style>