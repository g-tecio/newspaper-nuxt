<template>
  <b-container class="container-without-img">
    <h1>{{ article.title }}</h1>
    {{ article.content }}

    <div class="article-date">
      <b-row>
        <b-col md="8">Thursday February, 7</b-col>
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
        id: "194qxwEd104",
        title: "Times Are Changing",
        content: `This is a text without sense so don't waste time reading it it's just to see the article visual behaivor
                  This is a text without sense so don't waste time reading it it's just to see the article visual behaivor`,
        img: 30
      }
    }
  } 
}
</script>


<style>
.see-more {
  color: #d2222a !important;
}
.article-date {
  color: #a2a2a2;
}
.container-without-img {
  padding-top: 10px;
  padding-bottom: 10px;
}
</style>
