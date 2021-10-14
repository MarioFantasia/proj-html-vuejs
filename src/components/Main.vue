<template>
    <main>
        <div class="container">
            <SectionTop></SectionTop>
            <SectionTutoring></SectionTutoring>
            <SectionThree></SectionThree>
        </div>
            <SectionFour></SectionFour>
        <div class="container">
            <SectionLearning></SectionLearning>
        </div>
        <div class="bgc">
            <SectionCourses></SectionCourses>
            <SectionPricing></SectionPricing>
        </div>
        <div class="container">
            <SectionBottom></SectionBottom>
        </div>
    </main>
</template>

<script>
import SectionTop from './MainComponents/SectionTop.vue'
import SectionTutoring from './MainComponents/SectionTutoring.vue'
import SectionThree from './MainComponents/SectionThree.vue'
import SectionFour from './MainComponents/SectionFour.vue'
import SectionLearning from './MainComponents/SectionLearning.vue'
import SectionCourses from './MainComponents/SectionCourses.vue'
import SectionPricing from './MainComponents/SectionPricing.vue'
import SectionBottom from './MainComponents/SectionBottom.vue'
export default {
    name : 'Main',
    components : {
        SectionTop,
        SectionTutoring,
        SectionThree,
        SectionFour,
        SectionLearning,
        SectionCourses,
        SectionPricing,
        SectionBottom
    }
}
</script>

<style lang="scss" scoped>
    .bgc {
        background-image: url('../assets/img/main/background-pattern.jpg');
    }
</style>