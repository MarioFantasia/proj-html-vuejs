<template>
    <section>
        <div class="row">
            <ul class="col-3">
                <li class="program"  v-for="(elm, index) in programs" :key="index">{{elm}}</li>
            </ul>
            <div class="col-9">
                <div class="text">
                    <h2>Learning Possibilities</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus illum quaerat, magni ut quisquam assumenda eligendi in ipsam asperiores consequuntur nihil dolorem optio, quo vitae. Pariatur similique est laboriosam suscipit.</p>
                </div>
                <div class="info flex">
                    <div class="todo">
                        <div v-for="(elm, index) in actions" :key="index"><i class="fas fa-check"></i> {{elm}}</div>
                    </div>
                    <div class="image cflex">
                        <img src="../../assets/img/main/h12-tabs-icon-1.png" alt="img">
                    </div>
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
        padding: 50px 0;
        color: #847b7b;
        .row {
            height: 100%;
            .col-3 {
                height: 100%;
                padding: 0;
                border: 1px solid;
                border-bottom: 0;
                .program {
                    height: 70px;
                    line-height: 70px;
                    padding-left: 30px;
                    font-weight: 700;
                    border-bottom: 1px solid;
                    &:hover {
                        border-left: 5px solid #45c6ff;
                        background-color: #f2f2f2;
                    }
                }
            }

            .col-9 {
                height: 100%;
                .text {
                    height: 50%;
                    padding: 0 300px 0 30px;
                    h2 {
                        height:70px;
                        line-height:70px;
                        font-size: 40px;
                        font-weight: 500;
                        color: black;
                    }

                    p {
                        margin-bottom: 50px;
                    }

                }

                .info {
                    height: 50%;
                    padding-left: 30px;
                    .todo {
                        width: 70%;
                        height: 100%;
                        div {
                            margin-bottom: 30px;
                            i {
                                color: #45c6ff;
                            }
                        }
                    }

                    .image {
                        width: 30%;
                        height: 100%;
                        margin-top: auto;
                        img {
                            width: 50%;
                            height: 50%;
                            margin-right: auto;
                        }
                    }
                }
            }
        }
    }
</style>