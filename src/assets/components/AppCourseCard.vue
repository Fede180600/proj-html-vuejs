<template>
    <div class="my_card">
        <div class="img_container">
            <img :src="require(`../img/${courseCard.poster}`)" alt="">
            <span v-if="courseCard.special">special</span>
        </div>

        <div class="text">
            <h4>{{ courseCard.title }}</h4>
            <small>{{ courseCard.type }}</small>
        </div>

        <div class="container">
            <ul class="row row-cols-3  card_list">
                <li><i class="fas fa-signal"></i>{{ courseCard.level }}</li>
                <li><i class="fas fa-list"></i>{{ courseCard.lectures }}</li>
                <li><i class="fas fa-clock"></i>{{ courseCard.duration }}</li>
            </ul>
        </div>

    </div>
</template>

<script>

export default {
    name: 'AppCourseCard',
    props: {
        courseCard: Object
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";
.my_card {
    text-align: center;
    padding: 0;
    background-color: white;
    width: calc(100% / 3 - 20px);
    margin-bottom: 30px;
    .img_container {
        margin-bottom: 30px;
        position: relative;
        span {
            background-color: $brand-secondary-color;
            text-transform: uppercase;
            color: white;
            font-size: .6rem;
            font-weight: 800;
            border-radius: 5px;
            padding: 2px 5px;
            position: absolute;
            top: 10px; 
            right: 10px;
        }
    }
    .text {
        margin-bottom: 20px;
        h4 {
        font-size: 1.5rem;
        font-weight: 800;
        }
        small {
            font-family: 'Roboto', sans-serif;
            color: $app-light-gray;
        }
    }
    .card_list {
        border-top: 1px solid lightgray;
        padding: 10px 0 0 0;
        font-size: 12px;
        list-style: none;
        font-family: 'Roboto', sans-serif;
        color: $app-dark-gray;
        i {
            color: $brand-primary-color;
            font-size: 1rem;
            margin-right: 5px;
        }
    }
}
</style>