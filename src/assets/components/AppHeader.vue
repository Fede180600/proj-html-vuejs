<template>
    <header>
        <div class="my_container container d-flex justify-content-between align-items-center">
            <div class="logo-container" style="width: 20%;">
                <img src="../img/logo.png" alt="">
            </div>
            <nav class="d-flex">
                <ul class="d-flex justify-content-between align-items-center me-5 flex-grow-1">
                    <li v-for="item in headerNavItems" :key="item.id" style="position: relative;">
                        {{ item.content }}
                        <span v-if="item.new" style="position: absolute; top: -10px; right: -5px; background-color: #dc1245; color: white; border-radius: 5px; padding: 0 5px; font-size: 10px; text-transform: uppercase;">new</span>
                        <span v-else></span>
                    </li>
                    
                </ul>
                <div class="socials-container d-flex align-items-center" style="font-size: 600;">
                    <i class="fab fa-linkedin"></i>
                    <i class="fab fa-instagram"></i>
                    <i class="fab fa-facebook"></i>
                    <i class="fab fa-twitter"></i>
                </div>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    props: {
        headerNavItems: Array,
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

header {
    height: 100px;
    background-color: #ffffff;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 1000;
    width: 100%;
    .my_container {
        height: 100%;
        nav {
        width: 50%;
        ul {
            padding: 0;
            margin: 0;
            list-style: none;
            height: 40px;
            font-weight: 600;
            li {
                cursor: pointer;
            }
        }
        i {
            margin: 0 5px;
        }
    }
    }
}
</style>