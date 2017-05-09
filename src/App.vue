<template>
  <div id="app">
    <div class="layout">
      <app-top></app-top>
      <app-nav></app-nav>
      <router-view></router-view>
      <app-back-top></app-back-top>
      <div class="layout-copy">
        2011-2016 &copy; Claws Pet Vet
      </div>
    </div>
  </div>
</template>

<script>
import AppTop from '@/components/Top'
import AppNav from '@/components/Nav'
import AppBackTop from '@/components/BackTop'
export default {
  name: 'app',
  components: {
    'app-top': AppTop,
    'app-nav': AppNav,
    'app-back-top': AppBackTop
  },
  data () {
    return {
      theme1: 'light'
    }
  }
}
</script>

<style>
#app {
  font-family: "Helvetica Neue", "Luxi Sans", "DejaVu Sans", Tahoma, "Hiragino Sans GB", STHeiti, "Microsoft YaHei";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.ivu-menu li a{
  color: #657180;
}

</style>
