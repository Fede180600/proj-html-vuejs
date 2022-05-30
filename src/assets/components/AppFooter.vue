<template>
    <footer>
        <div class="container">
            <div class="row row-cols-4">
                <ul>
                    <h3>About</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est excepturi minus aut, similique at ab
                        corporis temporibus voluptates voluptate voluptatibus, vero dolores nesciunt ipsa voluptas cum
                        fugit sunt aliquam esse?</p>
                </ul>
                <ul>
                    <h3>contact</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est excepturi minus aut, similique at ab
                        corporis temporibus voluptates voluptate voluptatibus, vero dolores nesciunt ipsa voluptas cum
                        fugit sunt aliquam esse?</p>
                </ul>
                <ul>
                    <h3>pages</h3>
                    <div class="row row-cols-2">
                        <div>
                            <li>blog</li>
                            <li>home</li>
                            <li>shortcodes</li>
                        </div>

                        <div>
                            <li>courses</li>
                            <li>membership</li>
                            <li>typhography</li>
                        </div>
                    </div>

                </ul>
                <ul>
                    <h3>blog</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est excepturi minus aut, similique at ab
                        corporis temporibus voluptates voluptate voluptatibus, vero dolores nesciunt ipsa voluptas cum
                        fugit sunt aliquam esse?</p>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'AppFooter',
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

footer {
    padding: 40px 0;
    background-color: $brand-primary-color;
    border: 1px solid black;
}
</style>