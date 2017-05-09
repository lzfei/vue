<style scoped>
  .ivu-menu-horizontal.ivu-menu-light:after {
    height: 0;
  }
  .layout-logo{
    width: 190px;
    height: 30px;
    float: left;
    position: relative;
    top: 15px;
    left: 60px;
    font-size: 22px;
    color: #657180;
  }
  .layout-header{
    height: 60px;
    background: #fff;
    box-shadow: 0 1px 1px rgba(0,0,0,.1);
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
<template>
  <div class="layout-header">
    <Row>
      <Col span="5">
        <router-link to="/"><div class="layout-logo">Claws Pet Vet</div></router-link>
      </Col>
      <Col span="9">
        <Menu mode="horizontal">
          <Menu-item name="1">
            <router-link to="medicalBeauty">医疗美容</router-link>
          </Menu-item>
          <Menu-item name="2">
            <router-link to="petProducts">宠物用品</router-link>
          </Menu-item>
          <Submenu name="3">
            <template slot="title">
              <router-link to="record">档案记录</router-link>
            </template>
            <Menu-group title="使用">
              <Menu-item name="3-1">新增和启动</Menu-item>
              <Menu-item name="3-2">活跃分析</Menu-item>
              <Menu-item name="3-3">时段分析</Menu-item>
            </Menu-group>
            <Menu-group title="留存">
              <Menu-item name="3-4">用户留存</Menu-item>
              <Menu-item name="3-5">流失用户</Menu-item>
            </Menu-group>
          </Submenu>
          <Menu-item name="4">
            <router-link to="set">综合设置</router-link>
          </Menu-item>
        </Menu>
      </Col>
      <Col span="3"><Input class="cpv-search" placeholder="请输入..."></Input></Col>
      <Col span="1"><Button class="cpv-search-btn" type="primary" icon="ios-search">搜索</Button></Col>
      <Col span="6"><div class="cpv-call">联系电话：400-675-5462</div></Col>
    </Row>
  </div>
</template>
<script>
  export default {
    name: 'nav'
  }
</script>
