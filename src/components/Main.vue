<template>
    <main>
        <div class="container">
            <SectionTop></SectionTop>
            <SectionTutoring></SectionTutoring>
            <SectionThree></SectionThree>
        </div>
            <SectionFour></SectionFour>
        
        
    </main>
</template>

<script>
import SectionTop from './MainComponents/SectionTop.vue'
import SectionTutoring from './MainComponents/SectionTutoring.vue'
import SectionThree from './MainComponents/SectionThree.vue'
import SectionFour from './MainComponents/SectionFour.vue'
export default {
    name : 'Main',
    components : {
        SectionTop,
        SectionTutoring,
        SectionThree,
        SectionFour
    }
}
</script>

<style lang="scss" scoped>

</style>