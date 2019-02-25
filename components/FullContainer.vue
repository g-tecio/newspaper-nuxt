<template>
    <div class="news-container">
        <div class="primary-articles-full">
            <b-row>
                <b-col class="article-wrapper-right" md="6">
                    <ArticleLeftSide />
                </b-col>
                <b-col class="article-wrapper " md="6">
                    <ArticleRightSide />
                </b-col>
            </b-row>
        </div>
    </div>
</template>

<script>
import ArticleLeftSide from '~/components/articles/ArticleLeftSide.vue'
import ArticleRightSide from '~/components/articles/ArticleRightSide.vue'

export default {
    components: {
        ArticleLeftSide,
        ArticleRightSide
    }
}
</script>


<style>
    .primary-articles-full {
        border-top: 2px solid #000;
        height: 80% !important;
        padding-top: 10px;
    }
    .article-wrapper-right{
        border-right: 1px solid #000;
    }
 
</style>
