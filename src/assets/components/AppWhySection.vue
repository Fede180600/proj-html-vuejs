<template>
    <section class="why_section">
        <div class="container">
            <h2 style="text-align: center; margin-bottom: 50px; font-weight: 800; font-size: 2.8rem;">Why my Courses?</h2>
            <div class="row row-cols-2 justify-content-between">
                <AppWhyCard v-for="(why, index) in whyArray" :key="index" :whyCard="why"/>
            </div>
        </div> 
    </section>
</template>

<script>
import AppWhyCard from "./AppWhyCard.vue";

export default {
    name: 'AppWhySection',
    components: {
        AppWhyCard
    },
    props: {
        whyArray: Array
    }
}
</script>

<style lang="scss" scoped>
.why_section {
    padding: 60px 0;
}
</style>