<template>
    <div>
        <b-row>
            <b-col class="article-wrapper" md="6">
                <ArticleWithoutImg />
            </b-col>
            <b-col class="article-wrapper" md="6">
                <ArticleImg />
            </b-col>
            <b-col class="article-wrapper" md="6">
                <ArticleWithoutImg />
            </b-col>
            <b-col class="article-wrapper" md="6">
                <ComplexArticle />
            </b-col>
        </b-row>
        
    </div>
</template>

<script>
import ArticleImg from '~/components/articles/ArticleImg.vue'
import ComplexArticle from '~/components/articles/ComplexArticle.vue'
import ArticleWithoutImg from '~/components/articles/ArticleWithoutImg.vue'
export default {
    components: {
        ArticleWithoutImg,
        ArticleImg,
        ComplexArticle
    }
}
</script>


<style>
    .article-wrapper {
        display: inline-block;
        border-right: 2px solid #424242;
        border-right: 50%;
    }
</style>
