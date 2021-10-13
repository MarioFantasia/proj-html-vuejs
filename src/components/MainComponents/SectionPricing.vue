<template>
    <section>
        <div class="container">
            <div class="row">

                <div class="col-3">
                    <div class="box flex">
                        <h3 class="flex">Save up to 40% by paying weekly</h3>
                    </div>
                    <ul>
                        <li v-for="(elm, index) in indicator" :key="index">{{elm}}</li>
                    </ul>
                </div>

                <div class="col-3">
                    <div class="box box_image cflex">
                        <div class="image">
                            <img src="../../assets/img/main/h5-custom-icon-7.png" alt="">
                        </div>
                        <div class="type">Standard</div>
                        <div class="cost">$12</div>
                    </div>
                    <ul>
                        <li>2</li>
                        <li>15 DAYS</li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-times"></i></li>
                        <li><i class="fas fa-times"></i></li>
                        <li><i class="fas fa-times"></i></li>
                        <li><i class="fas fa-times"></i></li>
                    </ul>
                    <div class="button">
                        <button>GET IT NOW</button>
                    </div>
                </div>

                <div class="col-3">
                    <div class="box box_image cflex">
                        <div class="image">
                            <img src="../../assets/img/main/h5-custom-icon-7.png" alt="">
                        </div>
                        <div class="type">Standard</div>
                        <div class="cost">$12</div>
                    </div>
                    <ul>
                        <li>4</li>
                        <li>30 DAYS</li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-times"></i></li>
                        <li><i class="fas fa-times"></i></li>
                    </ul>
                    <div class="button">
                        <button>GET IT NOW</button>
                    </div>
                </div>

                <div class="col-3">
                    <div class="box box_image cflex">
                        <div class="image">
                            <img src="../../assets/img/main/h5-custom-icon-7.png" alt="">
                        </div>
                        <div class="type">Standard</div>
                        <div class="cost">$12</div>
                    </div>
                    <ul>
                        <li>6</li>
                        <li>30 DAYS</li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-check"></i></li>
                        <li><i class="fas fa-check"></i></li>
                    </ul>
                    <div class="button">
                        <button>GET IT NOW</button>
                    </div>
                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name : 'SectionPricing',
    data() {
        return {
            indicator : [
                'Numbers of Course',
                'Time',
                'Web Designing',
                'Human-Centered Design',
                'Basik Marketing',
                'Phyton for Everybody',
                'Android Developer',
                'Business English',
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    section {
        background-image: url('../../assets/img/main/background-pattern.jpg');
        .container {
            height: 100%;
            border: 1px solid #efefef;
            .col-3 {
                padding: 0;
            }
        }
    }

    .box {
        height: 250px;
        background-color: #fff;
        border: 1px solid #efefef;
    }
    
    ul {
        margin: 0;
    }

    li {
        height: 50px;
        background-color: #fff;
        border: 1px solid;
        text-align: center;
        line-height: 50px;
        border: 1px solid #efefef;
        .fa-check {
            color: #40c4ff;
        }

        .fa-times {
            color: #8f8f8f;
        }

    }

    h3 {
        margin: auto 0;
        text-align: center;
    }

    .box_image {
        text-align: center;
        justify-content: center;
    }

    .button {
        text-align: center;
        padding: 30px;
        background-color: #f7fdff;
        border: 1px solid #efefef;

        button {
            width: 100%;
            height: 60px;
            background-color: white;
            border: 1px solid #efefef;

        }
    }
</style>