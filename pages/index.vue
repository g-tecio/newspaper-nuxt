<template>
  <div>
    <Header />
    <Categories />
    <NewsBanner />
    <b-container>
      <b-row>
        <b-col md="9">
          <NewsContainer />
        </b-col>
        <b-col md="3">
          <SideNews />
        </b-col>
        <b-col md="12">
          <FullContainer />
        </b-col>
        <b-col md="9" class="after-col">
          <AfterFullContainer/>
        </b-col>
        <b-col md=3 class="after-col">
          <SideNews2/>
        </b-col>
        <b-col md="9" class="final-col">
          <NewsContainer2/>
        </b-col>
        <b-col md="3" class="final-col2">
          <SideNews3/>
        </b-col>
    </b-row>
    </b-container>
    
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Header from '~/components/Header.vue'
import Categories from '~/components/Categories.vue'
import NewsBanner from '~/components/NewsBanner.vue'
import NewsContainer from '~/components/NewsContainer.vue'
import SideNews from '~/components/SideNews.vue'
import FullContainer from '~/components/FullContainer.vue'
import AfterFullContainer from '~/components/AfterFullContainer.vue'
import SideNews2 from '~/components/SideNews2.vue'
import NewsContainer2 from '~/components/NewsContainer2.vue'
import SideNews3 from '~/components/SideNews3.vue'

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
    NewsContainer2,
    SideNews3
  }
}
</script>

<style>

  .title {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
      'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
  }

  .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }

  .links {
    padding-top: 15px;
  }

  .after-col{
    padding-top: 10px;
    padding-bottom: 10px;
  }

  .final-col{
    border-top: 2px solid #000;
    padding-top: 10px;
    padding-bottom: 10px;
  }

  .final-col2{
    border-top: 2px solid #000;
    padding-top: 10px;
    padding-bottom: 10px;
  }
</style>
