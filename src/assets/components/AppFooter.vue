<template>
    <footer>
        <div class="container">
            <div class="row row-cols-4">
                
                <AppFooterElement v-for="(item, index) in footerElementsArray" :key="index" :footerElement="item" />
                
            </div>
        </div>
    </footer>
</template>

<script>
import AppFooterElement from "./AppFooterElement.vue";
export default {
    name: 'AppFooter',
    props: {
        footerElementsArray: Array
    },
    components: {
        AppFooterElement
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

footer {
    padding: 40px 0;
    background-color: $brand-primary-color;
}
</style>