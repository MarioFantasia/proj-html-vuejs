<template>
    <section>
        <div class="row">
            <div class="col-8">
                <div class="image flex">
                    <img src="../../assets/img/main/h5-img-2.jpg" alt="img">
                </div>
            </div>
            <div class="col-4 cflex">
                <h2>Empowering Children to Reach Their Potential.</h2>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Facere necessitatibus molestias, sapiente laboriosam, id modi optio omnis minus ea, quidem beatae nihil. Alias iure ea sint cupiditate nostrum dignissimos reprehenderit.</p>
                <div class="row">

                    <div class="data col-5">
                        <h3>168</h3>
                        <h5>User Stories</h5>
                    </div>
                    <div class="data col-5">
                        <h3>347</h3>
                        <h5>Events</h5>
                    </div>

                </div>
            </div>
        </div>
    </section>
</template>

<script>

export default {
    name : 'SectionThree',
}
</script>

<style lang="scss" scoped>
    $principalColor : #40c4ff;
    section {
        .image {
            width: 100%;
            img {
                width: 70%;
                margin: 0 auto;
            }
        }

        h2, p {
            margin-bottom: 30px;
        }

        .data {
            color: $principalColor;
        }

        h3 {
            font-size: 50px;
        }
    }
</style>