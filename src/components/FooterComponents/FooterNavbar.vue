<template>
    <nav class="flex">

        <div class="first_col cflex col-3">
            <div class="logo flex">
                <img src="../../assets/img/footer/footer-logo-1.png" alt="logo">
            </div>

            <ul>
                <li v-for="(elm, index) in todos" :key="index">
                    <a href="#">{{elm}}</a>
                </li>
            </ul>
            <!-- modificare successivamente per inserire le fontawesome -->
            <div v-for="(elm, index) in infos" :key="index">
                <i :class="elm.icon"></i>
                <span>{{elm.info}}</span>
            </div>
        </div>

        <div class="col-3">
            <h3>Popular Courses</h3>
            <ul class="list_courses">
                <li  v-for="(elm, index) in courses" :key="index">
                    <a href="#">{{elm}}</a>
                </li>
            </ul>
        </div>

        <div class="support col-3">
            <h3>Support</h3>
            <ul>
                <li v-for="(elm, index) in supports" :key="index">
                    <a href="#">{{elm}}</a>
                </li>
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

            infos : [
                {
                    info: '1-677-124-44227',
                    icon :'fas fa-phone-alt'
                },
                
                {
                    info: 'Mon-Sat 8.00-18.00',
                    icon: 'far fa-clock'
                }
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
        a {
            color: #b9b9b9;
            &:hover {
                color: #3db5eb;
            } 
        }
    }

    h3 {
        margin-bottom: 20px;
        color: white;
    }

    .first_col li, .support li {
        margin-bottom: 10px;
    }

    .first_col i {
        margin-right: 10px;
    }

    .list_courses li:nth-child(odd) {
        font-size: 20px;
        font-weight: 500;
    }

    .list_courses li:nth-child(even) {
        margin-bottom: 20px;
    }

    .map {
        width: 100%;
        img {
            width: 70%;
        }
    }

</style>