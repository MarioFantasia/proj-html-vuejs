<template>
    <section>
        <div class="container">
            <div class="text cflex">
                <h2>Pricing Plans</h2>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptate quasi ipsum.</p>
            </div>
            <div class="row">
                <div class="col-3">
                    <div class="box flex">
                        <h3 class="flex">Save up to 40% by paying weekly</h3>
                    </div>
                    <ul>
                        <li class="classes" v-for="(elm, index) in indicator" :key="index">{{elm}}</li>
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
                            <img src="../../assets/img/main/h5-custom-icon-8.png" alt="">
                        </div>
                        <div class="type">Professional</div>
                        <div class="cost">$59</div>
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
                            <img src="../../assets/img/main/h5-custom-icon-9.png" alt="">
                        </div>
                        <div class="type">Advance</div>
                        <div class="cost">$88</div>
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
            ],
            standard : false,
            proifessional : false,
            advance : false
            
        }
    }
}
</script>

<style lang="scss" scoped>
    $principalColor : #40c4ff;
    $secondColor : #efefef;
    $threeColor : #f7fdff;
    $textColor : #8e8e8e;

    .row {
        border: 1px solid $secondColor;
        background-color: white;
        .col-3 {
            padding: 0;
            &:hover .box_image {
                border-top-color: $principalColor;
            }
        }
    }

    .text {
        height: 200px;
        text-align: center;
        padding: 0 100px;
        justify-content: center;
    }

    .box {
        height: 200px;
        border: 1px solid $secondColor;
        border-top: 3px solid #d6f2ff;
    }
    
    ul {
        margin: 0;
        color: $textColor;
    }

    li {
        border: 1px solid;
        text-align: center;
        line-height: 50px;
        font-weight: 500;
        border: 1px solid $secondColor;
        .fa-check {
            color: $principalColor;
        }

        .fa-times {
            color: #8f8f8f;
        }
    }

    .classes {
        font-weight: 800;
        font-family: 'Andada Pro', serif;
    }

    h3 {
        margin: auto 0;
        text-align: center;
    }

    .box_image {
        text-align: center;
        justify-content: center;
        background-color: $threeColor;
        font-size: 20px;
        font-weight: 700;
    }

    .type, .cost {
        font-family: 'Andada Pro', serif;
        font-weight: 800;
    }

    .button {
        text-align: center;
        padding: 30px;
        background-color: $threeColor;
        border: 1px solid $secondColor;

        button {
            width: 100%;
            height: 60px;
            color: $textColor;
            font-weight: 700;
            background-color: white;
            border: 1px solid $secondColor;
            &:hover {
                color: white;
                background-color: $principalColor;
            }
        }
    }
</style>