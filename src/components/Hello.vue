<style scoped>
  .layout-1200{
    width: 1200px;
    margin: 0 auto;
  }
  .f1{
    margin-top: 50px;
    height: 350px;
  }
  .f1-left{
    width: 600px;
    height: 350px;
    float: left;
    padding-top: 38px;
    padding-left: 100px;
    text-align: left;
  }
  .title{
    font-size: 35px;
    padding-bottom: 15px;
  }
  .sub-title{
    font-size: 25px;
    list-style: disc;
    padding-top: 15px;
    color: #39f;
  }
  .des{
    font-size: 18px;
    color: #999;
    line-height: 28px;
  }
  .f2{
    margin-top: 50px;
    height: 350px;
  }
  .f2-left{
    float: left;
    padding-left: 150px;
    width: 600px;
  }
  .f2-right{
    float: right;
    text-align: left;
    padding-right: 150px;
    padding-top: 50px;
  }
</style>
<template>
  <div>
    <Carousel autoplay v-model="value2"
              :autoplay-speed="setting.autoPlaySpeed"
              :height="setting.height">
      <Carousel-item>
        <div class="demo-carousel">
          <img src="../assets/image/carousel-1.jpg"/>
        </div>
      </Carousel-item>
      <Carousel-item>
        <div class="demo-carousel">
          <img src="../assets/image/carousel-2.jpg"/>
        </div>
      </Carousel-item>
      <Carousel-item>
        <div class="demo-carousel">
          <img src="../assets/image/carousel-3.jpg"/>
        </div>
      </Carousel-item>
    </Carousel>
    <div class="layout-1200 f1">
      <ul class="f1-left">
        <li class="title">专业爱宠医疗美容</li>
        <li class="sub-title">宠物医疗</li>
        <li class="des">专业医师，为爱宠去除病痛</li>
        <li class="sub-title">宠物美容</li>
        <li class="des">职业美容医师，让您的小可爱光彩照人</li>
      </ul>
      <img class="f1-right" src="../assets/image/hello/hello-1.jpg"/>
    </div>
    <div class="layout-1200 f2">
      <img class="f2-left" src="../assets/image/hello/hello-2.jpg"/>
      <ul class="f2-right">
        <li class="title">宠物日常用品大全</li>
        <li class="sub-title">宠物饲料、玩具、衣物</li>
        <li class="des">物美价廉，品质有保障</li>
      </ul>
    </div>
    <div class="layout-1200 f1">
      <ul class="f1-left">
        <li class="title">健康档案及饲养建议</li>
        <li class="sub-title">健康状况统计</li>
        <li class="des">建立爱宠健康档案，关注他们的健康</li>
        <li class="sub-title">合理化建议</li>
        <li class="des">专业饲养建议，安全省心</li>
      </ul>
      <img class="f1-right" src="../assets/image/hello/hello-3.jpg"/>
    </div>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        value2: 0,
        setting: {
          autoPlaySpeed: 3000,
          height: 550
        }
      }
    }
  }
</script>

