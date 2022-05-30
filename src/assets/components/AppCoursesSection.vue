<template>
    <section style="background-color: #e4e7e7; padding: 50px 0; ">
        <div class="container">
            <h2 style="text-align: center; margin-bottom: 30px;">New Courses</h2>
            <div class="row row-cols-3 justify-content-between">
                <AppCourseCard />
                <AppCourseCard />
                <AppCourseCard />
                <AppCourseCard />
                <AppCourseCard />
                <AppCourseCard />
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
    }
}
</script>

<style lang="scss" scoped>
</style>