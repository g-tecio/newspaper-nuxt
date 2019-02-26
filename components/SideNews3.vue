<template>
    <div class="side-news">
        <SideArticle3 class="side-article3"/>
    </div>
</template>

<script>
import SideArticle3 from '~/components/articles/SideArticle3.vue'
export default {
    components: {
        SideArticle3
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