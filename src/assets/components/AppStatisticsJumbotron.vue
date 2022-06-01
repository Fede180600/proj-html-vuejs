<template>
<section class="statistics_jumbotron">
    <div class="container">
        <ul class="row row-cols-4">
            <li v-for="(item, index) in statisticsArray" :key="index" class="d-flex align-items-center">
                <i :class="item.icon"></i>
                <div class="item_text">
                    <h2>{{ item.number }}</h2>
                    <p>{{ item.text }}</p>
                </div>
            </li>
        </ul>
    </div>
</section>
</template>

<script>

export default {
    name: 'AppStatisticsJumbotron',
    props: {
        statisticsArray: Array
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

.statistics_jumbotron {
    background-image: url(../img/counter-1919x1101.jpg);
    background-position: top;
    background-size: cover;
    padding: 200px 0;
    ul {
        list-style: none;
        color: white;
        i {
            font-size: 3.5rem;
            margin-right: 20px;
        }
        h2 {
            margin-bottom: 0;
            font-weight: 800;
            color: $brand-primary-color;
        }
    }
}
</style>