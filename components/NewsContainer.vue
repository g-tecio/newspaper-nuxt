<template>
    <div class="news-container">
        <div class="primary-articles-container">
            <b-row class="row-primary">
                <b-col class="article-wrapper-left" md="6">
                    <ArticleWithoutImg />
                </b-col>
                <b-col class="article-wrapper" md="6">
                    <ArticleImg />
                </b-col>
            </b-row>
        </div>
        <div class="seconday-articles">
            <b-row>
                <b-col class="article-wrapper-left" md="6">
                    <ArticleWithoutImg />
                </b-col>
                <b-col class="article-wrapper" md="6">
                    <ComplexArticle />
                </b-col>
            </b-row>
        </div>
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

    @media screen and (max-width: 548px) {
        
        .news-container {
            padding: 8%;
        }
    }
    .primary-articles-container {
        border-bottom: 1px solid gray;
    }
    .row-primary{
        padding-bottom: 10px;
    }
    .seconday-articles {
        padding-top: 10px;
        padding-bottom: 10px;
    }
    .article-wrapper-left{
        border-right: 1px solid gray;
    }

</style>
