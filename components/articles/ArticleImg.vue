<template>
    <b-container class="container-img">

        <b-img class="article-img" src="https://picsum.photos/1024/400/?image=41" fluid alt="Responsive image"/>
        <p class="p-font">{{ article.content }}</p>

        <div class="article-date">
            <b-row>
                <b-col md="8">
                    Thursday February, 7
                </b-col>
                <b-col class="text-right" md="4">
                    <b-link class="see-more text-right" :key="article.id" :to="{ name: 'article-id', params: { id: article.id, title: article.title, content: article.content, img: article.img } }">See more...</b-link>
                </b-col>
            </b-row>  
        </div>

    </b-container>
</template>

<script>
export default {
  data() {
    return {
      article: {
        id: "9796qxwEd981273",
        title: "Another testing title",
        content: `Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis sed purus ullamcorper, rutrum lacus vitae, sollicitudin augue. 
                Proin rhoncus facilisis eros vel vestibulum. Nulla facilisi. Donec eu ex sed nulla congue imperdiet. Nulla facilisi. 
                Quisque eleifend aliquet metus, tempor sodales neque condimentum sit amet. Aenean eu viverra lorem, 
                sit amet eleifend erat. In suscipit hendrerit libero vitae auctor. Curabitur nibh nisl, egestas a nisl at, luctus eleifend sem`,
        img: 41
      }
    }
  } 
}
</script>

<style>
    .p-font{
        font-size: 18px;
    }
    .see-more {
        color: #D2222A !important;
    }
    .article-date {
        color: #A2A2A2;
    }
    .article-img {
        width: 100%;
        height: 260px !important;
    }
    .container-img{
        padding-top: 10px;
        padding-bottom: 10px;
    }
</style>
