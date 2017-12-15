<template>
  <div id="app">
    <v-header></v-header>
    <p>
      <router-link to="/">首页</router-link>
      <router-link to="/about">关于我们</router-link>
      <router-link to="/service">服务项目</router-link>
      <router-link to="/news">聚城新闻</router-link>
      <router-link to="/case">聚城案例</router-link>
      <router-link to="/contact">联系我们</router-link>
    </p>
    <router-view></router-view>
    <v-footer></v-footer>
</div>
</template>

<script>
import Vheader from '@/components/header/header';
import Vfooter from '@/components/footer/footer';
export default {
  components: {
       'v-header': Vheader,
       'v-footer': Vfooter
   }
};
</script>

<style>
#app {
  width: 500px;
  margin: auto;
}
</style>
