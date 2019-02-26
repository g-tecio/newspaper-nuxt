<template>
    <div class="news-container2">
        <div class="primary-articles-container2">
            <b-row class="row-primary">
                <b-col class="article-wrapper-left2" md="6">
                    <ArticleWithoutImg />
                </b-col>
                <b-col class="article-wrapper2" md="6">
                    <ArticleImg />
                </b-col>
            </b-row>
        </div>
    </div>
</template>

<script>
import ArticleImg from '~/components/articles/ArticleImg.vue'
import ArticleWithoutImg from '~/components/articles/ArticleWithoutImg.vue'
export default {
    components: {
        ArticleWithoutImg,
        ArticleImg,
    }
}
</script>


<style>
    .primary-articles-container2{
        padding-top: 10px;
    }

</style>