<template>
    <div class="side-news">
        <SideArticle class="side-article"/>
        <SideArticle class="side-article"/>
        <SideArticle class="side-article"/>
        <SideArticle class="side-article"/>
        <SideArticle class="side-article"/>
    </div>
</template>

<script>
import SideArticle from '~/components/articles/SideArticle.vue'
export default {
    components: {
        SideArticle
    }
}
</script>

<style>
    .side-news {
        border-left: #424242 solid 1px;
    }
    .side-article{
        padding-bottom: 10px;
    }
</style>


