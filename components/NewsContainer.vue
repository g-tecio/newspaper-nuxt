<template>
    <div class="news-container">
        <div class="primary-articles">
            <b-row>
                <b-col class="article-wrapper " md="6">
                    <ArticleWithoutImg />
                </b-col>
                <b-col class="article-wrapper " md="6">
                    <ArticleImg />
                </b-col>
            </b-row>
        </div>
        <div class="seconday-articles">
            <b-row>
                <b-col class="article-wrapper" md="6">
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
        .article-wrapper {
            border-right: none !important;
            border-bottom: #424242 solid 1px;
        }
        .primary-articles {
            border-bottom: none !important;
        }

        .news-container {
            padding: 8%;
        }
    }
    
    .article-wrapper {
        display: inline-block;
        border-right: 2px solid #898989;
        border-right: 50%;
    }

    .primary-articles {
        border-bottom: 2px solid #898989;
        height: 80% !important;
    }
    .secondary-articles {
        height: 20% !important;
    }

</style>
