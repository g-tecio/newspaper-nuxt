<template>
    <b-container class="container-complex">
        <b-row>
            <b-col md="7">
                <h3>{{ article.title }}</h3>
                <p>{{ article.content }}</p>
            </b-col>
            <b-col md="5">
                <b-img class="article-img-complex" :src='"https://picsum.photos/1024/400/?image=" + article.img' fluid alt="Responsive image"/>
            </b-col>
            <b-col md="6" class="article-date">
                    Thursday February, 7
            </b-col>
            <b-col class="text-right" md="6">
                <b-link class="see-more text-right" :key="article.id" :to="{ name: 'article-id', params: { id: article.id, title: article.title, content: article.content, img: article.img } }">See more...</b-link>
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
export default {
  data() {
    return {
      article: {
        id: "801DePxLk129",
        title: "News About Chairs",
        content: `Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis sed purus ullamcorper, rutrum lacus vitae, sollicitudin augue. 
                Proin rhoncus facilisis eros vel vestibulum. Nulla facilisi. Donec eu ex sed nulla congue imperdiet. Nulla facilisi. 
                Quisque eleifend aliquet metus, tempor sodales neque condimentum sit amet. Aenean eu viverra lorem, 
                sit amet eleifend erat. In suscipit hendrerit libero vitae auctor. Curabitur nibh nisl, egestas a nisl at, luctus eleifend sem`,
        img: 42
      }
    }
  } 
}
</script>

<style>
    b-container{
        padding-top: 10px;
    }
    .see-more {
        color: #D2222A !important;
    }
    .article-date {
        color: #A2A2A2;
    }
    .article-img-complex {
        width: 100%;
        height: 215px;
        max-height: 215px;
    }
    .container-complex{
        padding-top: 10px;
        padding-bottom: 10px;
    }
</style>