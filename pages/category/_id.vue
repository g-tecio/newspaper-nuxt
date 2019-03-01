<template>
  <div>
    <Header/>
    <Categories/>
    <NewsBanner/>
    <b-container>
      <b-row>
        <b-col md="4">
          <h1 class="category-title">{{ $route.params.id }}</h1>
        </b-col>
      </b-row>
      <b-row>
        <b-col class="category-container" md="4">
          <b-container class="container-img category-main-art">
            <b-img
              class="article-img"
              :src="'https://picsum.photos/1024/400/?image=' + $route.params.img"
              fluid
              alt="Responsive image"
            />
            <h2>This article is for the {{ $route.params.id }} category</h2>
            <div class="article-date">
              <b-row>
                <b-col md="8">Thursday February, 7</b-col>
                <b-col class="text-right" md="4">
                  <b-link class="see-more text-right" href="#">See more...</b-link>
                </b-col>
              </b-row>
            </div>
          </b-container>

          <b-container class="category-main-art">
            <ArticleWithoutImg/>
          </b-container>
        </b-col>

        <b-col class="border-bottom" md="8">
          <b-row>
            <b-col class="border-right" md="8">
              <b-container class="container-img category-main-art">
                <b-img
                  class="article-img"
                  :src="'https://picsum.photos/1024/400/?image=' + $route.params.img + 1"
                  fluid
                  alt="Responsive image"
                />
                <h2>This module is an intro to a full article of {{ $route.params.id }}</h2>
                <div class="article-date">
                  <b-row>
                    <b-col md="8">Thursday February, 7</b-col>
                    <b-col class="text-right" md="4">
                      <b-link class="see-more text-right" href="#">See more...</b-link>
                    </b-col>
                  </b-row>
                </div>
              </b-container>
            </b-col>
            <b-col class="border-bottom" md="4">
              <SideArticle/>
              <SideArticle/>
              <SideArticle/>
            </b-col>

            <b-col md="12">
              <ComplexArticle/>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
      <b-row>
        <b-col md="4">
          <h5 class="category-title"><strong>Latest</strong></h5>
        </b-col>
      </b-row>
      <b-row>
        <b-col md="12">
          <AfterFullContainer/>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";
import Header from "~/components/Header.vue";
import Categories from "~/components/Categories.vue";
import NewsBanner from "~/components/NewsBanner.vue";
import NewsContainer from "~/components/NewsContainer.vue";
import ArticleWithoutImg from "~/components/articles/ArticleWithoutImg.vue";
import ComplexArticle from "~/components/articles/ComplexArticle.vue";
import SideArticle from "~/components/articles/SideArticle.vue";
import SideNews from "~/components/SideNews.vue";
import FullContainer from "~/components/FullContainer.vue";
import AfterFullContainer from "~/components/AfterFullContainer.vue";
import SideNews2 from "~/components/SideNews2.vue";
export default {
  components: {
    Logo,
    Header,
    Categories,
    NewsBanner,
    NewsContainer,
    SideNews,
    FullContainer,
    AfterFullContainer,
    SideNews2,
    ArticleWithoutImg,
    SideArticle,
    ComplexArticle
  },
  data() {
    return {};
  },
  validate({ params }) {
    // Must be a number
    return params.id;
  }
};
</script>

<style>
.border-right {
  border-right: 1px #565656 solid;
}
.border-bottom {
  border-bottom: 1px #565656 solid;
}

.category-container {
  border-right: 1px #565656 solid;
}
.category-title {
  border-block-end: 1px #565565 solid;
  margin-top: 20px;
}

.category-main-art {
  border-bottom: #565565 solid 1px;
}

.see-more {
  color: #d2222a !important;
}
.article-date {
  color: #a2a2a2;
}
.article-img {
  width: 100%;
  height: 260px;
}
.container-img {
  padding-top: 10px;
  padding-bottom: 10px;
}
</style>

