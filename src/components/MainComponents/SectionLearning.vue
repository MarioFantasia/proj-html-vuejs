<template>
    <section>
        <div class="row">
            <div class="col-3"></div>
            <div class="col-9">
                <div class="text"></div>
                <div class="info flex">
                    <div class="todo"></div>
                    <div class="image"></div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name : 'SectionLearning',
    data() {
        return {
            programs : [
                'What We Do',
                'Degree Programme',
                'Carrer Archievements',
                'Personal Managment',
                'Steps To Success',
                'Knowledge Transfer',
            ],

            actions : [
                'We enrich lives throught learning.',
                'Maximizin potential throught individual attention.',
                'The trusted name.',
                'People teach. People learn. This is where they connect.',
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    section {
        height: 100vh;
        padding: 50px 0;
        .row {
            height: 100%;
            .col-3 {
                height: 100%;
                background-color: red;
            }
            .col-9 {
                height: 100%;
                background-color: blue;
                .text {
                    height: 50%;
                    background-color: green;
                }
                .info {
                    height: 50%;
                    background-color: grey;
                    .todo {
                        width: 70%;
                        height: 100%;
                        background-color: pink;
                    }
                    .image {
                        width: 30%;
                        height: 100%;
                        background-color: orange;
                    }
                }
            }
        }
    }
</style>