<template>
    <section>
        <div class="container">
            <div class="text cflex">
                <h2>Popular Online Courses</h2>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Explicabo nostrum provident distinctio nam perferendis deleniti amet consectetur quidem eos nisi, quod ducimus, consequatur officiis rerum quasi, necessitatibus ullam vel! Modi.</p>
            </div>
            <div class="card_items row">
                <div class="box col-4" v-for="(elm, index) in cards" :key="index">
                    <Card :element="elm "></Card>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import Card from './SectionCoursesComponent/Card.vue'
export default {
    name : 'SectionCourses',
    components : {
        Card
    },

    data() {
        return {
            cards: [
                {
                    course: 'Android Developer',
                    picture : 'course-5-f-img.jpg',
                    teacher: 'David Sanders',
                    value: 'FREE',
                    description : 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repudiandae quos cum consequuntur animi praesentium neque expedita dolor mollitia quibusdam fugit temporibus.',
                    type: 'Programming'
                },
                {
                    course: 'Web Designing',
                    picture : 'course-6-f-img.jpg',
                    teacher: 'Jennifer Powell',
                    value: 'FREE',
                    description : 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repudiandae quos cum consequuntur animi praesentium neque expedita dolor mollitia quibusdam fugit temporibus.',
                    type: 'Programming'
                },
                {
                    course: 'Financial Modelling',
                    picture : 'course-12-f-img.jpg',
                    teacher: 'Edward Bowman',
                    value: '$20',
                    description : 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repudiandae quos cum consequuntur animi praesentium neque expedita dolor mollitia quibusdam fugit temporibus.',
                    type: 'Programming'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .text {
        height: 200px;
        text-align: center;
        justify-content: center;
        h2, p {
            margin-bottom: 30px;
            padding: 0 100px;
        }
    }
</style>