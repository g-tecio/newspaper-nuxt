<template>
    <div class="side-news">
        <SideArticle2 class="side-article2"/>
    </div>
</template>

<script>
import SideArticle2 from '~/components/articles/SideArticle2.vue'
export default {
    components: {
        SideArticle2
    }
}
</script>

<style>
    .side-news {
        border-left: #424242 solid 1px;
    }
    .side-article2{
        padding-top: 10px;
        padding-bottom: 10px;
    }
</style>
