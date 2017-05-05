<template>
  <div id="app">
    <div class="layout">
      <div class="layout-ceiling">
        <div class="layout-ceiling-main">
          <a href="#">注册登录</a> |
          <a href="#">帮助中心</a> |
          <a href="#">安全中心</a> |
          <a href="#">服务大厅</a>
        </div>
      </div>
      <div class="layout-header">
        <Row>
          <Col span="6"><div class="layout-logo">Claws Pet Vet</div></Col>
          <Col span="6"><Input class="cpv-search" placeholder="请输入..."></Input></Col>
          <Col span="2"><Button class="cpv-search-btn" type="primary" icon="ios-search">搜索</Button></Col>
          <Col span="10"><div class="cpv-call">联系电话：400-675-5462</div></Col>
        </Row>

      </div>
      <router-view></router-view>
      <div class="layout-copy">
        2011-2016 &copy; Claws Pet Vet
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.layout{
  background: #f5f7f9;
  position: relative;
  overflow: hidden;
}
.layout-logo{
  width: 190px;
  height: 30px;
  float: left;
  position: relative;
  top: 15px;
  left: 60px;
  font-size: 22px;
}
.layout-header{
  height: 60px;
  background: #fff;
  box-shadow: 0 1px 1px rgba(0,0,0,.1);
}
.layout-copy{
  text-align: center;
  padding: 10px 0 20px;
  color: #9ea7b4;
}
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
.cpv-search{
  top:15px;
}
.cpv-search-btn{
  top:15px;
  position: relative;
  float: left;
  margin-left: 5px;
}
.cpv-call{
  top:15px;
  height: 30px;
  vertical-align: middle;
  position: relative;
  font-size: 18px;
}
</style>
