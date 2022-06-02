<template>
    <section style="background-color: #edf2f5; padding: 60px 0; ">
        <div class="container text-center">
            <h2 style="text-align: center; margin-bottom: 50px; font-size: 2.8rem; font-weight: 800;">New Courses</h2>
            <div class="row row-cols-3 justify-content-between">
                <AppCourseCard v-for="(card, index) in coursesArray" :key="index" :courseCard="card"/>
            </div>
            <button>Load More</button>
        </div>
    </section>
</template>

<script>
import AppCourseCard from "./AppCourseCard.vue";
export default {
    name: 'AppCoursesSection',
    components: {
        AppCourseCard
    },
    props: {
        coursesArray: Array
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";
button {
    font-family: 'roboto' sans-serif;
    text-transform: uppercase;
    color: white;
    font-size: .8rem;
    font-weight: 600;
    background-color: $brand-primary-color;
    border: none;
    border-radius: 50px;
    padding: 10px 20px;
}
button:hover {
    background-color: rgb(221, 144, 0);
}
</style>