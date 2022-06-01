<template>
    <div class="why_card">
        <i :class="whyCard.icon"></i> 
        <h3>{{ whyCard.title }}</h3>
        <p>{{ whyCard.text }}</p>
    </div>
</template>

<script>

export default {
    name: 'AppWhyCard',
    props: {
        whyCard: Object
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";
.why_card {
    position: relative;
    width: calc(100% / 2 - 20px);
    margin-bottom: 30px;
    padding: 40px 80px;
    border-left: 6px solid $brand-primary-color;
    -webkit-box-shadow: 0px 0px 13px 4px #85858596;
    -moz-box-shadow: 0px 0px 13px 4px #85858596;
    -o-box-shadow: 0px 0px 13px 4px #85858596;
    box-shadow: 0px 0px 13px 4px #85858596;
    i {
        position: absolute; 
        top: 40px; left: 20px; 
        font-size: 2.5rem; 
        color: $brand-primary-color;
    }
    h3 {
        font-weight: 800;
        margin-bottom: 15px;
    }
    p {
        color: $app-light-gray;
        font-size: .9rem;
        line-height: 25px;
    }
}
</style>