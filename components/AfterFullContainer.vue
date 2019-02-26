<template>
    <div class="news-container">
        <div class="primary-articles-2">
            <b-row>
                <b-col class="article-wrapper-right" md="6">
                    <ArticleWithoutImg />
                </b-col>
                <b-col class="article-wrapper-mini" md="3">
                    <ArticleWithoutImg2 />
                </b-col>
                <b-col class="article-wrapper-mini2" md="3">
                    <ArticleWithoutImg2 />
                </b-col>
            </b-row>
        </div>
    </div>
</template>

<script>

import ArticleWithoutImg from '~/components/articles/ArticleWithoutImg.vue'
import ArticleWithoutImg2 from '~/components/articles/ArticleWithoutImg2.vue'


export default {
    components: {
        ArticleWithoutImg,
        ArticleWithoutImg2
    }
}
</script>

<style>
    .article-wrapper-right{
        padding-top: 10px;
    }
    .article-wrapper-mini{
        border-right: 1px solid #000;
        padding-top: 10px;
    }
    .article-wrapper-mini2{
        padding-top: 10px;
    }
</style>