<template>
    <main>
        <div class="container">
            <SectionTop></SectionTop>
            <SectionTutoring></SectionTutoring>
            <SectionThree></SectionThree>
        </div>
    </main>
</template>

<script>
import SectionTop from './MainComponents/SectionTop.vue'
import SectionTutoring from './MainComponents/SectionTutoring.vue'
import SectionThree from './MainComponents/SectionThree.vue'
export default {
    name : 'Main',
    components : {
        SectionTop,
        SectionTutoring,
        SectionThree
    }
}
</script>

<style lang="scss" scoped>

</style>