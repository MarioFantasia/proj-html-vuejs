<template>
    <main>
        <div class="container">
            <SectionTop></SectionTop>
            <SectionTutoring></SectionTutoring>
        </div>
    </main>
</template>

<script>
import SectionTop from './MainComponents/SectionTop.vue'
import SectionTutoring from './MainComponents/SectionTutoring.vue'
export default {
    name : 'Main',
    components : {
        SectionTop,
        SectionTutoring
    }
}
</script>

<style lang="scss" scoped>

</style>