<template>
    <nav class="flex">

        <div class="first_col cflex col-3">
            <div class="logo flex">
                <img src="../../assets/img/footer/footer-logo-1.png" alt="logo">
            </div>

            <ul>
                <li v-for="(elm, index) in todos" :key="index">{{elm}}</li>
            </ul>
            <!-- modificare successivamente per inserire le fontawesome -->
            <div v-for="(elm, index) in infos" :key="index">{{elm}}</div>
        </div>

        <div class="list_courses col-3">
            <h3>Popular Courses</h3>
            <ul>
                <li  v-for="(elm, index) in courses" :key="index">{{elm}}</li>
            </ul>
        </div>

        <div class="col-3">
            <h3>Support</h3>
            <ul>
                <li  v-for="(elm, index) in supports" :key="index">{{elm}}</li>
            </ul> 
        </div>

        <div class="col-3">
            <h3>Flexible Learning</h3>
            <div class="map">
                <img src="../../assets/img/footer/footer-img-1.png" alt="map">
            </div>
        </div>

    </nav>
</template>

<script>
export default {
    name : 'FooterNavbar',
    data() {
        return {
            todos : [
                'Providing Life Changing',
                'Experiences Through',
                'Education. Class That Fit Your',
                'Busy Life. Closer to Home'
            ],

            icons : [
                /* mettere i codici delle fontawesome */
            ],

            infos : [
                '1-677-124-44227',
                'Mon-Sat 8.00-18.00'
            ],

            courses : [
                'Business English',
                'Preston Marshall',
                'Social Computing',
                'David Sanders',
                'Learn Spanish',
                'Jennie King',
            ],

            supports : [
                'User dashboard',
                'Contact Us',
                'FAQ',
                'Course Offer',
                'Events',
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
    nav {
        justify-content: space-between;
        .logo {
            width: 150px;
            margin: 2px 0 25px 0;
            img {
                width: 100%;
            }
        }
    }
    h3 {
            margin-bottom: 20px;
    }

    .map {
        width: 100%;
        img {
            width: 70%;
        }
    }

</style>