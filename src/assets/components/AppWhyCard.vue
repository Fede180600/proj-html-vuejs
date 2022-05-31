<template>
    <div class="why_card">
        <h3>Entrepreneurship</h3>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Adipisci fugit iure recusandae ex natus excepturi consequatur, aperiam ipsam molestias eius praesentium nostrum corporis similique. Nobis nesciunt nemo molestias harum ipsum.</p>
    </div>
</template>

<script>

export default {
    name: 'AppWhyCard',
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";
.why_card {
    width: calc(100% / 2 - 20px);
    margin-bottom: 30px;
    border: 1px solid black;
    -webkit-box-shadow: 0px 0px 13px 4px #85858596;
    -moz-box-shadow: 0px 0px 13px 4px #85858596;
    -o-box-shadow: 0px 0px 13px 4px #85858596;
    box-shadow: 0px 0px 13px 4px #85858596;

    // TEST
    padding: 20px 60px;
}
</style>