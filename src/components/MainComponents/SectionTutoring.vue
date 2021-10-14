<template>
    <section>
        <div class="box">
            <h2>The Trusted Name for In-Home Tutoring.</h2>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nesciunt voluptas neque sapiente aperiam ullam officia, laudantium nobis delectus, perferendis consectetur itaque aspernatur quo sit consequatur illo culpa architecto recusandae? Deleniti!</p>
            <a href="#">LEARN MORE</a>
            <div class="image flex">
                <img src="../../assets/img/main/h5-img-1.jpg" alt="">
            </div>
        </div>
    </section>
</template>

<script>

export default {
    name : 'SectionTutoring'
}
</script>

<style lang="scss" scoped>
    $principalColor : #3db5eb;
    section {
        h2 {
            width: 45%;
            font-size: 40px;
            font-weight: 500;
        }

        h2, p {
            margin-bottom: 30px;
        }

        a {
            color: $principalColor;
            font-weight: 500;
        }

        .image{
            width: 100%;
            img {
                width: 70%;
                margin: 0 auto;
            }
        }
    }
    
</style>