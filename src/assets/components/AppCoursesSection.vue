<template>
    <section style="background-color: #edf2f5; padding: 60px 0; ">
        <div class="container">
            <h2 style="text-align: center; margin-bottom: 50px; font-size: 2.8rem; font-weight: 800;">New Courses</h2>
            <div class="row row-cols-3 justify-content-between">
                <AppCourseCard v-for="(card, index) in coursesArray" :key="index" :courseCard="card"/>
            </div>
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
</style>