<!--首页最后一个页面，广告宣传页-->

<template>
  <div id="home-ad">
    <div class="ad-map">
      <p class="title">复瑛健康——蛋白质医学研发网络</p>
      <p class="content">三个计算中心 亿级存储计算能力，万级并发服务能力</p>
      <p class="content">三个检测中心 十万级检测能力</p>
      <p class="content">九个队列中心 万级样本</p>
      <img src="~assets/img/home/map.png">
    </div>
    <div class="ad-company">
      <p class="title">复瑛健康-合作伙伴（部分单位，排名不分先后）</p>
      <div id="university">
        <img src="~assets/img/home/university/Harvard.png" @click="goPage('https://www.harvard.edu/')">
        <img src="~assets/img/home/university/Johns Hopkins.png" @click="goPage('https://www.jhu.edu/')">
        <img src="~assets/img/home/university/Baylor.png" @click="goPage('https://www.bcm.edu/')">
        <img src="~assets/img/home/university/Mayo.png" @click="goPage('https://mandarin.mayoclinic.org/')">
        <img src="~assets/img/home/university/Stanford.png" @click="goPage('https://www.stanford.edu/')">
        <img src="~assets/img/home/university/Tsinghua.png" @click="goPage('https://www.tsinghua.edu.cn/')">
        <img src="~assets/img/home/university/Fudan.png" @click="goPage('https://www.fudan.edu.cn/')">
        <img src="~assets/img/home/university/Fudan-ZL.png" @click="goPage('https://www.shca.org.cn/')">
        <img src="~assets/img/home/university/Zhejiang.png" @click="goPage('http://www.zy91.com/index/index.jhtml')">
        <img src="~assets/img/home/university/ZhongShan.png" @click="goPage('http://www.zs-hospital.sh.cn/')">
        <!-- <img src="~assets/img/home/university.png"> -->
      </div>
      <div class="right-text">
        <p class="title">复瑛健康拥有专业的保密团队，通过硬件以及流程管理等各方面保护用户数据，
        建立完整的隐私保护体系。我们承诺对受检者个人系统账号、个人信息、与蛋白质信息给予严格保密，除非得到您
        本人的确认，不会透露给第三方</p>
        <button @click="buyClick">Try it now</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeAd",
  methods: {
    buyClick() {
      this.$router.replace("/products")
    },
    goPage(url) {
      window.location.href = url
    }
  }
}
</script>

<style scoped>
  .ad-map, .ad-company{
    width: var(--screen-width);
    text-align: center;
  }
  .ad-company{
    background: url("~assets/img/bg/doctor.png") no-repeat;
  }
  #university{
    height: 380px;
    width: 620px;
    margin-left: auto;
    margin-right: auto;
  }
  #university img{
    cursor: pointer;
  }
  .ad-map .title{
    padding-bottom: 30px;
  }
  .ad-map .content{
    text-align: left;
    margin-left: 750px;
  }
  .ad-map img, .ad-company img{
    padding-top: 20px;
  }
  .right-text{
    width: 760px;
    margin-left: 700px;
    margin-top: var(--div-bottom);
    line-height: 50px;
  }
  button {
    background-color: #ffce6b;
    border: none;
    color: #6b6b6b;
    padding: 15px 50px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 24px;
    font-weight: bold;
    cursor: pointer;
}
</style>