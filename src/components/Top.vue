<style scoped>
  .layout-ceiling{
    background: #464c5b;
    padding: 10px 0;
    overflow: hidden;
  }
  .layout-ceiling-main{
    float: right;
    margin-right: 15px;
  }
  .layout-ceiling-main a{
    color: #9ba7b5;
  }
</style>
<template>
  <div class="layout-ceiling">
    <div class="layout-ceiling-main" v-for="m in menus">
      <!--使用v-for遍历-->
      <router-link :to="setPath(m.path)"><span>{{m.text}}</span></router-link>
    </div>
  </div>
</template>
<script>
  export default {
    name: 'top',
    data () {
      return {
        // top部分顶部参数
        menus: [{
          text: '注册登录',
          path: '/'
        }, {
          text: '帮助中心',
          path: '/'
        }, {
          text: '安全中心',
          path: '/'
        }, {
          text: '服务大厅',
          path: '/'
        }]
      }
    },
    methods: {
      setPath (path) {
        return path
      }
    }
  }
</script>
