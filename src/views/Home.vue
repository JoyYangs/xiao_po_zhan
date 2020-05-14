<template>
  <div class="home">
    <home-header></home-header>
    <navigation-bar class="nav-bar" :titles="titles"></navigation-bar>
    <home-content class="content"></home-content>
  </div>
</template>

<script>
// @ is an alias to /src
import NavigationBar from '@/components/NavigationBar.vue'
import HomeHeader from '@/views/Header.vue'
import NavTop from '@/components/NavTop.vue'
import HomeContent from './Content.vue'

export default {
  name: 'Home',
  components: {
    NavigationBar,
    HomeHeader,
    NavTop,
    HomeContent
  },
  data() {
    return {
      titles: {
        left: ["主站","番剧","游戏中心","直播","会员购","漫画","赛事","下载APP"],
        right: ["大会员","消息","动态","收藏","历史","创作中心"]
      }
    }
  }
}
</script>

<style scoped>
.nav-bar {
  position: absolute;
  left: 0px;
  top: 0px;
  background-color: rgba(255, 255, 255, 0);
}

.content {
  /* background-color: aqua; */
  margin: 0 60px;
  height: 1000px;
}
</style>
