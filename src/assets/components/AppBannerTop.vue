<template>
    <div class="banner">
        <div class="banner_top">
            <div class="container">
                <div class="banner_text">
                    <h2>
                        Start Your Human
                        <br>
                        <span class="text_brand_primary_color">Revolution</span>
                        Today
                    </h2>
                    <p>A wonderful serenity taken possession of my entire soul, like these sweet mornings of spring which i enjoy with my whole heart</p>
                </div>

            </div>
        </div>

        <div class="banner_middle">
            <h2><h2 style="color: white;">Limited Sale:</h2> All Courses with 55% off</h2>
            <br>
            <input type="text" placeholder="Enter your E-mail">
            <button>subscribe</button>
            <div class="countdown_container d-flex justify-content-between" style=";">
                <div class="countdown_box" v-for="(item, index) in countdown" :key="index">
                    <h3>{{ item.number }}</h3>
                    <small>{{ item.description }}</small>
                </div>
            </div>
        </div>

        <div class="banner_bottom">
            <div class="container">
                <div class="row row-cols-2 justify-content-center">
                    <div
                        style="width: 40%; display: flex; flex-direction: column; justify-content: center; align-items: center;">
                        <h2>Hi there, my name is Jhon Doe, I'm the founder of the Brain Accademy.</h2>
                        <img src="../img/sign.jpg" alt="firma Jhon Doe" style="width: 30%; margin-top: 20px;">
                    </div>
                    <div>
                        <p>
                            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Perferendis voluptatibus ullam a
                            ducimus quidem, molestiae aut officiis aliquam eum tenetur facilis aliquid nihil deleniti et
                            quam quibusdam praesentium commodi sed. Lorem ipsum dolor sit amet consectetur adipisicing
                            elit. Expedita sequi sed aut labore sint tempora accusamus cumque laborum beatae tenetur,
                            nisi aspernatur sit odio ipsum, odit, eos nulla praesentium ullam! Lorem ipsum dolor sit
                            amet consectetur adipisicing elit.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'AppBannerTop',
    props: {
        countdown: Array
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

.banner {
    position: relative;

    &_top {
        background-image: url(../img/slide-1.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        // height: 900px;
        padding: 400px 0;
        margin-top: 100px;

        .banner_text {
            width: 25%;
            position: absolute;
            top: 20%;
            right: 14vw;
            transform: translate(-50%, -50%);
            h2 {
                font-weight: 800;
                font-size: 3.2rem;
            }
            p {
                font-size: 1rem;
                color: #363636;
            }
        }
    }

    &_middle {
        height: 200px;
        width: 68%;
        padding: 30px 80px;
        background-color: $brand-primary-color;
        position: absolute;
        left: 50%;
        top: 45%;
        transform: translate(-50%, 50%);
        border-radius: 10px;
        h2 {
            margin-bottom: 15px;
            display: inline-block;
            font-size: 1.9rem;
            font-weight: 800;
        }
        input,
        button {
            padding: 15px 20px;
            border: 0;
            outline: none;
            border-radius: 50px;
            font-size: .9rem;
        }
        input {
            width: 40%;
        }
        button {
            position: relative;
            right: 40px;
            background-color: #2d4649;
            text-transform: uppercase;
            color: white;
        }
        .countdown_container {
            position: relative;
            bottom: 60px;
            float: right; 
            width: 40%;
            .countdown_box {
                text-align: center;
                margin-left: 10px;
                h3 {
                font-size: 3.8rem;
                font-weight: 800;
                color: white;
                }
                small {
                    font-weight: 800;
                }
            }
        }
    }

    &_bottom {
        padding: 150px 0 100px 0;
        h2 {
            font-size: 2.2rem;
            font-weight: 800;
        }
        p {
            line-height: 30px;
            font-family: 'Roboto', sans-serif;
        }
    }
}
</style>