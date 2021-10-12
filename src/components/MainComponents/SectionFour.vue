<template>
    <section class="flex">
        <div class="container">
            <div class="box">
                <div class="image">
                    <img src="../../assets/img/main/testimonials-standard-2.png" alt="testimonial">
                </div>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Cupiditate ad ullam praesentium iste dolorem veniam corporis sit vitae sint sequi neque natus alias consectetur, tempora non perferendis. Eius, earum voluptates.</p>
                <h4>Joan Collins</h4>
                <h5>Student</h5>
            </div>
        </div>
    </section>
</template>

<script>

export default {
    name : 'SectionFour',

}
</script>

<style lang="scss" scoped>
    section {
        height: 100vh;
        background-image: url('../../assets/img/main/h5-parallax-img-1.png');
        background-size: cover;
        background-position: top;
        .container {
            text-align: center;
            margin: auto;
            .box {
                color: white;
            }
        }
        .image, p {
            margin-bottom: 30px;
        }

        .image img {
            width: 10%;
        }

        p {
            font-size: 18px;
            padding: 0 300px;
        }
    }

</style>