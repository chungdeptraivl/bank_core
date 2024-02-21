<template>
  <div class="wrapper" style="display: flex; flex-direction: column">
    <!-- Banner and menu -->
    <div style="margin-top: 4px">
      <div style="position: relative">
        <home-banner />
        <menu-home
          style="
            position: absolute;
            top: 90%;
            left: 50%;
            transform: translateX(-50%);
          "
        />
      </div>
    </div>

    <!-- news -->
    <div style="margin-top: 8vw"><news-home /></div>

    <!-- jumbotron -->
    <div style="margin: 6vw 0"><jumbotron-home /></div>
  </div>
</template>

<script>
import HomeBanner from '~/components/home/homeBanner.vue'
import JumbotronHome from '~/components/home/jumbotronHome.vue'
import MenuHome from '~/components/home/menuHome.vue'
import NewsHome from '~/components/home/newsHome.vue'
export default {
  name: 'IndexPage',

  components: { HomeBanner, MenuHome, NewsHome, JumbotronHome },
}
</script>
