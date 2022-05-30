<template>
    <div class="banner">
        <div class="banner_top"></div>
    
        <div class="banner_middle"></div>

        <div class="banner_bottom">
            <div class="container">
                <div class="row row-cols-2">
                    <div style="border: 1px solid black; width: 45%; display: flex; flex-direction: column; justify-content: center;">
                        <h2>Hi there, my name is Jhon Doe, I'm the founder of the Brain Accademy</h2>
                        <img src="../img/sign.jpg" alt="firma Jhon Doe">
                    </div>
                    <div>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Perferendis voluptatibus ullam a ducimus quidem, molestiae aut officiis aliquam eum tenetur facilis aliquid nihil deleniti et quam quibusdam praesentium commodi sed. Lorem ipsum dolor sit amet consectetur adipisicing elit. Expedita sequi sed aut labore sint tempora accusamus cumque laborum beatae tenetur, nisi aspernatur sit odio ipsum, odit, eos nulla praesentium ullam! Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores porro omnis corrupti minima nobis cum ratione laboriosam officiis velit laudantium perferendis repellat veniam temporibus ullam quidem aliquam, culpa, provident expedita!</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'AppBannerTop'
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

.banner {
    position: relative;

    // TEST
    background-color: orangered;
    &_top {
        height: 600px;
        border: 1px solid white;
    }
    &_middle {
        height: 200px;
        width: 90%;
        background-color: $brand-primary-color;
        position: absolute;
        left: 50%;
        top: 30%;
        transform: translate(-50% , 50%);
        border-radius: 10px;
    }
    &_bottom {
        padding: 200px 0 50px 0;
    }
}
</style>