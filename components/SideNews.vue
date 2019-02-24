<template>
    <div class="side-news">
        <SideArticle />
        <SideArticle />
        <SideArticle />
        <SideArticle />
        <SideArticle />
        <SideArticle />
        <SideArticle />
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
</style>


