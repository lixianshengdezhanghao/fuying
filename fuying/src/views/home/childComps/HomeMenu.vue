<!--首页第三个页面，提供服务菜单-->

<template>
  <div id="home-menu">
    <p class="title">复瑛健康——探索人类健康的专家</p>
    <p class="content">选择复瑛，我们将会定期给你发送检测报告，实时监测您的健康状态。根据蛋白信息为您定制更系统的生活方案。让肌体保持青春，让生活更加舒适。</p>
    <div class="menu-lists">
      <icon-rectangle link="/intro"><img src="~assets/img/common/detect.png" slot="img"><p class="content" slot="text">检测流程</p></icon-rectangle>
      <icon-rectangle link="/login"><img src="~assets/img/common/report.png" slot="img"><p class="content" slot="text">检测报告</p></icon-rectangle>
      <icon-rectangle link="/"><img src="~assets/img/common/earphone.png" slot="img"><p class="content" slot="text">检测流程</p></icon-rectangle>
    </div>
    <div class="menu-lists">
      <icon-rectangle link="/login"><img src="~assets/img/common/cart.png" slot="img"><p class="content" slot="text">购物订单</p></icon-rectangle>
      <icon-rectangle link="/"><img src="~assets/img/common/file.png" slot="img"><p class="content" slot="text">检测实例</p></icon-rectangle>
      <icon-rectangle link="/intro"><img src="~assets/img/common/find.png" slot="img"><p class="content" slot="text">检测问答</p></icon-rectangle>
    </div>
  </div>
</template>

<script>
import IconRectangle from 'common/icon/IconRectangle'

export default {
  name: "HomeMenu",
  components: {
    IconRectangle,
  }
}
</script>

<style scoped>
  #home-menu{
    width: var(--screen-width);
    text-align: center;
    padding-bottom: var(--div-bottom);
  }
  .content{
    padding-bottom: var(--div-bottom);
  }
  .menu-lists{
    width: 850px;
    height: 300px;
    display: flex;
    margin-left: auto;
    margin-right: auto;
  }
</style>