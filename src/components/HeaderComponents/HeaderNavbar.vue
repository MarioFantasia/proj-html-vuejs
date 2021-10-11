<template>
    <nav class="flex col-10">
        <div class="link" v-for="(elm, index) in voces" :key="index">
            <a href="#">{{elm}}</a>
        </div>
        <div class="flex col-2 ">
            <i class="icon col" v-for="(elm, index) in icons" :key="index" :class="elm"></i>
        </div>
    </nav>
</template>

<script>
export default {
    name : 'HeaderNavbar',
    data() {
        return {
            voces : [
                'HOME',
                'COURSES',
                'INSTRUCTORS',
                'EVENTS',
                'PAGES',
                'ELEMENTS'
            ],

            icons : [
                'fas fa-search',
                'fas fa-shopping-bag',
                'fas fa-bars'
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    nav {
        height: 90%;
        margin: auto 0;
        color: white;
        justify-content: flex-end;
        .link {
            margin-left: 50px;
        }
        .link, i {
            text-align: right;
            /* altezza di nav è 90% di header_top "80px" */
            line-height: calc(80px * 0.9); 
        }
    }
</style>