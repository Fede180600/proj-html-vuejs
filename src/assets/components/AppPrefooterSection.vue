<template>
    <section class="prefooter_section">
        <div class="container">
            <div class="row align-items-center flex-column">
                <h3 style="font-size: 2.8rem; font-weight: 800;">What Students Say</h3>
                <div class="students_small_slider d-flex justify-content-between align-items-center">
                    <i class="fas fa-arrow-left"></i>
                    <div class="users_box d-flex align-items-center">
                        <div class="user"><img src="../img/1-100x100.jpg" alt=""></div>
                        <div class="user active"><img src="../img/2-100x100.jpg" alt=""></div>
                        <div class="user"><img src="../img/4-100x100.jpg" alt=""></div>
                    </div>
                    <i class="fas fa-arrow-right"></i>
                </div>
                <strong style="font-size: 1.4rem;">Paints of the Future</strong>
                <div class="stars">
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                </div>
                <p style="width: 50%;">
                The response to your MasterStudy has been really overwhelming! Those who participated 
                in the workshop are spreading the word here on campus and the "buzz" is on. The VP of 
                Instruction wants you to come back! Her goal is to have more faculty trained. She also 
                wants to attend a workshop herself. Our President told me Masterstudy needs to be the 
                cornerstone of our success program."
                </p>
            </div>
            
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppPrefooterSection',
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";
.prefooter_section {
    padding: 80px 0;
    text-align: center;
    .students_small_slider {
        height: 60px;
        width: 35%;
        min-width: 350px;
        margin: 20px 0;
        .user {
            height: 55px;
            width: 55px;
            border-radius: 50%;
            overflow: hidden;
            margin: 0 5px;
        }
        .user.active {
            height: 75px;
            width: 75px;
        }
    }
    .stars {
        color: $brand-primary-color;
        margin-bottom: 25px;
        i {
            margin: 0 2px;
        }
    }
    p {
        font-family: 'Roboto', sans-serif;
    }
}
</style>