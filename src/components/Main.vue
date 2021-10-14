<template>
    <main>
        <a href="#" class="up_page cflex">
            <i class="fas fa-chevron-up"></i>
            <div>TOP</div>
        </a>
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
    $principalColor : #40c4ff;
    .up_page {
        width: 50px;
        height: 50px;
        font-size: 12px;
        text-align: center;
        background-color: $principalColor;
        position: fixed;
        bottom: 15px;
        right: 0;
        cursor: pointer;
        justify-content: center;
        color: white;
    }
    .bgc {
        background-image: url('../assets/img/main/background-pattern.jpg');
    }
</style>