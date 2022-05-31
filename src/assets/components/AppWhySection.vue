<template>
    <section class="why_section">
        <div class="container">
            <h2 style="text-align: center; margin: 40px 0;">Why my Courses?</h2>
            <div class="row row-cols-2 justify-content-between">
                <AppWhyCard />
                <AppWhyCard />
                <AppWhyCard />
                <AppWhyCard />
            </div>
        </div> 
    </section>
</template>

<script>
import AppWhyCard from "./AppWhyCard.vue";

export default {
    name: 'AppWhtSection',
    components: {
        AppWhyCard
    }
}
</script>

<style lang="scss" scoped>
</style>