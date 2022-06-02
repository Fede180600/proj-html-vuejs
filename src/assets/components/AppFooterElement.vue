<template>
    <div>
        <ul>
            <h3>{{ footerElement.title }}</h3>
            <p>{{ footerElement.text }}</p>
            <div v-if="footerElement.icons" class="socials">
                <i v-for="(icon, index) in footerElement.icons" :key="index" :class="icon"
                    style="margin-right: 15px;"></i>
            </div>

            <p>{{ footerElement.address }}</p>
            <p v-if="footerElement.tel">Tel.:{{ footerElement.tel }}</p>
            <p v-if="footerElement.fax">Fax:{{ footerElement.fax }}</p>
            <p>{{ footerElement.email }}</p>

            <li v-for="(item, index) in footerElement.list" :key="index">{{ item }}</li>

            <div class="article d-flex" v-for="(article, index) in footerElement.articles" :key="index">
                <div class="article_img" style="width: 60%; margin-bottom: 20px; margin-right: 10px;">
                    <img :src="require(`../img/${article.poster}`)" alt="">
                </div>
                <p class="article_text">

                    <strong>{{ article.article_title }}</strong>
                    <br>
                    <small>
                        {{ article.date }}
                    </small>

                </p>
            </div>
        </ul>
    </div>
</template>

<script>
export default {
    name: "AppFooterElement",
    props: {
        footerElement: Object
    }
}
</script>

<style lang="scss" scoped>
h3 {
    text-transform: uppercase;
    font-size: 20px;
    font-weight: 800;
}

.article {
    align-items: center;
    min-width: 250px;

    small {
        color: gray;

    }

}

p {
    font-family: 'Roboto', sans-serif;
    font-size: 14px;

    strong {
        font-family: 'Roboto Slab', sans-serif;
        line-height: 0;
    }
}
</style>