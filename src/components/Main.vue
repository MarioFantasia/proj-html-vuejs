<template>
    <main>
        <div class="container">
            <SectionTop></SectionTop>
            <SectionTutoring></SectionTutoring>
            <SectionThree></SectionThree>
        </div>
            <SectionFour></SectionFour>
        <div class="container">
            <!-- altre sezioni -->
            <SectionBottom></SectionBottom>
        </div>
        
    </main>
</template>

<script>
import SectionTop from './MainComponents/SectionTop.vue'
import SectionTutoring from './MainComponents/SectionTutoring.vue'
import SectionThree from './MainComponents/SectionThree.vue'
import SectionFour from './MainComponents/SectionFour.vue'
/* altre sezioni */
import SectionBottom from './MainComponents/SectionBottom.vue'
export default {
    name : 'Main',
    components : {
        SectionTop,
        SectionTutoring,
        SectionThree,
        SectionFour,
        /* altre sezioni */
        SectionBottom
    }
}
</script>

<style lang="scss" scoped>

</style>