<template>
  <div>
    <Header/>
    <Categories/>
    <NewsBanner/>
    <br>
    <b-container>
      <b-row>
        <ArticleViewCard :content="$route.params"/>
        <b-col md="9">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis sed purus ullamcorper, rutrum lacus vitae, sollicitudin augue. Proin rhoncus facilisis eros vel vestibulum. Nulla facilisi. Donec eu ex sed nulla congue imperdiet. Nulla facilisi. Quisque eleifend aliquet metus, tempor sodales neque condimentum sit amet. Aenean eu viverra lorem, sit amet eleifend erat. In suscipit hendrerit libero vitae auctor. Curabitur nibh nisl, egestas a nisl at, luctus eleifend sem</p>
          <br>
          <p>Vivamus id sollicitudin massa, vitae bibendum ipsum. Sed finibus neque eu enim convallis, et convallis tortor porta. Integer consequat commodo risus quis posuere. Quisque bibendum erat quis nulla lobortis gravida. Suspendisse potenti. Curabitur eget ullamcorper dui. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Integer quis ligula non ex ullamcorper maximus. Aliquam convallis, nisl eu cursus imperdiet, risus odio sodales magna, non sollicitudin mi ex eu est. Vivamus commodo enim at est tincidunt dapibus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nulla maximus sollicitudin sem, quis tempus eros ultrices non. Suspendisse eget mauris erat. Sed nec eros at lectus tristique fermentum a a elit.</p>
          <br>
          <p>Vivamus id sollicitudin massa, vitae bibendum ipsum. Sed finibus neque eu enim convallis, et convallis tortor porta. Integer consequat commodo risus quis posuere. Quisque bibendum erat quis nulla lobortis gravida. Suspendisse potenti. Curabitur eget ullamcorper dui. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Integer quis ligula non ex ullamcorper maximus. Aliquam convallis, nisl eu cursus imperdiet, risus odio sodales magna, non sollicitudin mi ex eu est. Vivamus commodo enim at est tincidunt dapibus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nulla maximus sollicitudin sem, quis tempus eros ultrices non. Suspendisse eget mauris erat. Sed nec eros at lectus tristique fermentum a a elit.</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis sed purus ullamcorper, rutrum lacus vitae, sollicitudin augue. Proin rhoncus facilisis eros vel vestibulum. Nulla facilisi. Donec eu ex sed nulla congue imperdiet. Nulla facilisi. Quisque eleifend aliquet metus, tempor sodales neque condimentum sit amet. Aenean eu viverra lorem, sit amet eleifend erat. In suscipit hendrerit libero vitae auctor. Curabitur nibh nisl, egestas a nisl at, luctus eleifend sem</p>
          <br>
          <p>Vivamus id sollicitudin massa, vitae bibendum ipsum. Sed finibus neque eu enim convallis, et convallis tortor porta. Integer consequat commodo risus quis posuere. Quisque bibendum erat quis nulla lobortis gravida. Suspendisse potenti. Curabitur eget ullamcorper dui. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Integer quis ligula non ex ullamcorper maximus. Aliquam convallis, nisl eu cursus imperdiet, risus odio sodales magna, non sollicitudin mi ex eu est. Vivamus commodo enim at est tincidunt dapibus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nulla maximus sollicitudin sem, quis tempus eros ultrices non. Suspendisse eget mauris erat. Sed nec eros at lectus tristique fermentum a a elit.</p>
          <br>
          <p>Vivamus id sollicitudin massa, vitae bibendum ipsum. Sed finibus neque eu enim convallis, et convallis tortor porta. Integer consequat commodo risus quis posuere. Quisque bibendum erat quis nulla lobortis gravida. Suspendisse potenti. Curabitur eget ullamcorper dui. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Integer quis ligula non ex ullamcorper maximus. Aliquam convallis, nisl eu cursus imperdiet, risus odio sodales magna, non sollicitudin mi ex eu est. Vivamus commodo enim at est tincidunt dapibus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nulla maximus sollicitudin sem, quis tempus eros ultrices non. Suspendisse eget mauris erat. Sed nec eros at lectus tristique fermentum a a elit.</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis sed purus ullamcorper, rutrum lacus vitae, sollicitudin augue. Proin rhoncus facilisis eros vel vestibulum. Nulla facilisi. Donec eu ex sed nulla congue imperdiet. Nulla facilisi. Quisque eleifend aliquet metus, tempor sodales neque condimentum sit amet. Aenean eu viverra lorem, sit amet eleifend erat. In suscipit hendrerit libero vitae auctor. Curabitur nibh nisl, egestas a nisl at, luctus eleifend sem</p>
          <br>
          <p>Vivamus id sollicitudin massa, vitae bibendum ipsum. Sed finibus neque eu enim convallis, et convallis tortor porta. Integer consequat commodo risus quis posuere. Quisque bibendum erat quis nulla lobortis gravida. Suspendisse potenti. Curabitur eget ullamcorper dui. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Integer quis ligula non ex ullamcorper maximus. Aliquam convallis, nisl eu cursus imperdiet, risus odio sodales magna, non sollicitudin mi ex eu est. Vivamus commodo enim at est tincidunt dapibus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nulla maximus sollicitudin sem, quis tempus eros ultrices non. Suspendisse eget mauris erat. Sed nec eros at lectus tristique fermentum a a elit.</p>
          <br>
        </b-col>
        <b-col md="3" class="side-new">
          <SideNews/>
          <SideNews2/>
        </b-col>
        <b-col>
          <p style="font-weight :bold">More of this section</p>
        </b-col>
        <b-row class="new-container-row">
          <b-col class="new-container-1" md="5">
            <ArticleWithoutImg/>
          </b-col>
          <b-col class="new-container-2" md="5">
            <ArticleWithoutImg/>
          </b-col>
        </b-row>
      </b-row>
    </b-container>
    <FooterPage />
  </div>
</template>
<style>
.icons {
  float: right;
  width: 20px;
  height: 20px;
  display: inline-block;
}
.h1 {
  font-family: Merriweather;
}
.avatar {
  vertical-align: middle;
  width: 30px;
  height: 30px;
  border-radius: 50%;
  display: inline-block;
}

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
  /*
  width: 400%;
  height: 260px;
  */
  width: 375px;
  height: 700px;
}
.container-img {
  padding-top: 10px;
  padding-bottom: 10px;
}
</style>
<script>
import ArticleViewCard from "~/components/articles/ArticleViewCard.vue";
import FooterPage from "~/components/FooterPage.vue";
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
    ComplexArticle,
    ArticleViewCard,
    FooterPage
  },
  data() {
    return {};
  },
  validate({ params }) {
    return params.id;
  }
};
</script>



