<template>
    <section>
        <div class="row">
            <div class="col flex" v-for="(elm, index) in images" :key="index">
                <div class="work cflex">
                    <div class="box">
                        <!-- require necessario per visualizzare le immagini -->
                        <img :src="require('../../assets/img/main/h5-custom-icon-' + elm.num + '.png')" alt="alt">
                        <div>{{elm.name}}</div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name : 'SectionTop',
    data() {
        return {
            images : [
                {
                    num: '1',
                    name: 'Languages'
                },
                {
                    num: '2',
                    name: 'Software'
                },
                {
                    num: '3',
                    name: 'Business'
                },
                {
                    num: '4',
                    name: 'Chemistry'
                },
                {
                    num: '5',
                    name: 'Science'
                },
                {
                    num: '6',
                    name: 'DIY&Craft'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .row {
        justify-content: space-between;
    }
    .work {
        width: 100%;
        height: 150px;
        margin: auto;
        &:hover {
            background-color: #f2f8fc;
        }
        .box {
            margin: auto;
            text-align: center;
            font-weight: 500;
            img {
                margin-bottom: 10px;
            }

            div {
                font-size: 20px;
                font-weight: 700;
            }
        }
    }

</style>
