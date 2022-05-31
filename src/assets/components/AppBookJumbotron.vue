<template>
    <div class="banner_bottom">
    <div class="container">
        <img src="../img/book.png" alt="" style="width: 25%; max-width: 700px; min-width: 430px; position: absolute; bottom: 0; right: 12%; ">
        <div class="banner_text">
            <h2>Get my exclusive investing book just for $19.50</h2>
            <i>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores ipsam similique laudantium, recusandae vero nam ex deleniti perspiciatis, animi sed odio exercitationem velit molestiae reiciendis. Sapiente atque modi quis tenetur?</i>
        </div>
    </div>
    </div>
</template>

<script>

export default {
    name: 'AppBookJumbotron'
}
</script>

<style lang="scss" scoped>
.banner_bottom {
    background-image: url(../img/slider_1-1917x607-1914x606.jpg);
    background-size: cover;
    // height: 520px;
    padding-top: 500px;
    position: relative;
    .banner_text {
        // width: 30%;
        max-width: 350px;
        border: 1px solid white;
        text-align: center;
        position: absolute;
        left: 40%;
        top: 50%;
        transform: translate(-50%, -50%);
    }
}
</style>