<template>
    <div class="banner_bottom">
    <div class="container">
        <img src="../img/book.png" alt="" style="width: 25%; max-width: 450px; min-width: 440px; position: absolute; bottom: 0; right: 12%; ">
        <div class="banner_text">
            <h2 class="text_brand_primary_color">Get My Exclusive Investing Book just for $19.50</h2>
            <i>
                Vestibulum imentum eu urna vel cursus. Aenean 
                vehicula quam quam, vitae pellentesque urna 
                elementum cursus. 
            </i>
            
            <div><img src="../img/amazon.png" alt="" style="width: 40%; margin-top: 20px;"></div>
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
        max-width: 450px;
        text-align: center;
        position: absolute;
        left: 40%;
        top: 50%;
        transform: translate(-50%, -50%);
        h2 {
            font-weight: 600;
            margin-bottom: 20px;
        }
        i {
            color: white;
            font-size: 1.2rem;
            font-family: 'Roboto', sans-serif;
        }
    }
}
</style>