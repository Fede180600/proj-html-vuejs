<template>
    <div class="my_card">
        <div class="img_container">
            <img :src="require(`../img/${courseCard.poster}`)" alt="">
        </div>

        <div class="text">
            <h5>{{ courseCard.title }}</h5>
            <small>{{ courseCard.type }}}</small>
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

.my_card {
    text-align: center;
    padding: 0;
    background-color: white;
    width: calc(100% / 3 - 20px);
    margin-bottom: 30px;
    .card_list {
        border-top: 1px solid lightgray;
        padding: 10px 0 0 0;
        font-size: 12px;
        list-style: none;
    }
}
</style>