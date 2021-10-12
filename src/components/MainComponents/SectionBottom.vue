<template>
    <section class="flex">
            <div class="row row-cols-5">
                <div class="image" v-for="(elm, index) in images" :key="index">
                    <img class="out_hover" :src="require('../../assets/img/main/'+ elm.defaulf)" alt="img">
                    <img class="on_hover" :src="require('../../assets/img/main/'+ elm.onHover)" alt="img">
                </div>
            </div>
    </section>
</template>

<script>

export default {
    name : 'SectionBottom',
    data() {
        return {
            images : [
                {
                    defaulf : 'h5-client-1.png',
                    onHover : 'h5-client-1-h.png'
                },
                {
                    defaulf : 'h5-client-2.png',
                    onHover : 'h5-client-2-h.png'
                },
                {
                    defaulf : 'h5-client-3.png',
                    onHover : 'h5-client-3-h.png'
                },
                {
                    defaulf : 'h5-client-4.png',
                    onHover : 'h5-client-4-h.png'
                },
                {
                    defaulf : 'h5-client-5.png',
                    onHover : 'h5-client-5-h.png'
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
    section {
        height: 200px;
        .row {
            margin: auto 0;
        }
        .on_hover {
                display: none;
            }
        .image:hover .out_hover{
            display: none;
        }
        .image:hover .on_hover {
            display: block;
        }

    }
</style>