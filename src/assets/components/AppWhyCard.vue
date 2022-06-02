<template>
    <div class="why_card">
        <div class="yellow_border"></div>
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
    width: calc(100% / 2 - 10px);
    min-height: 300px;
    border: 15px solid none;
    margin-bottom: 30px;
    padding: 40px 80px;
    -webkit-box-shadow: 0px 0px 13px 4px #85858596;
    -moz-box-shadow: 0px 0px 13px 4px #85858596;
    -o-box-shadow: 0px 0px 13px 4px #85858596;
    box-shadow: 0px 0px 13px 4px #85858596;
    .yellow_border {
        width: 6px;
        height: 100%;
        background-color: $brand-primary-color;
        position: absolute;
        top: 0;
        left: 0;
    }
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
        font-family: 'Roboto', sans-serif;
        color: $app-light-gray;
        font-size: .9rem;
        line-height: 25px;
    }
}
.why_card:hover {
    background-color: $brand-primary-color;
    border: 15px solid white;
    p {
        color: black;
    }
    i {
        color: white;
    }
}
</style>