<template>
    <div class="my_card">
        <div class="img_container">
            <img src="../img/photo-1496307042754-b4aa456c4a2d-370x200.jpeg" alt="">
        </div>

        <div class="text">
            <h5>How to be a DJ? Make Elettronic Music</h5>
            <small>Electronic</small>
        </div>

        <div class="container">
            <ul class="row row-cols-3  card_list">
                <li><i class="fas fa-signal"></i></li>
                <li><i class="fas fa-list"></i></li>
                <li><i class="fas fa-clock"></i></li>
            </ul>
        </div>

    </div>
</template>

<script>

export default {
    name: 'AppCourseCard',
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