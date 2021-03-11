<template>
  <div class="site-footer flex-column">
    <div class="flex-row page-bottom-top">
      <div class="site-top-logo">
        <img
          src="https://xl.linkstars.com/asset/img/xingluo-components/xingluo-components-page-bottom-logo.png"
        />
      </div>
      <div>
        <div class="site-bottom-fa">
          <div class="site-bottom">
            <span class="site-bottom-title">导航</span>
            <a href="https://www.linkstars.com/" class="site-bottom-link"
              >首页</a
            >
            <a
              href="https://www.haohuo.com"
              target="_blank"
              class="site-bottom-link"
              >电商带货平台</a
            >
            <a
              href="https://xl.linkstars.com/solutions/services"
              class="site-bottom-link"
              >品牌抖音/快手全案服务</a
            >
            <a
              href="https://openapi.linkstars.com/doc/home/"
              target="_blank"
              class="site-bottom-link"
              >开放平台</a
            >
          </div>
          <div class="site-bottom">
            <span class="site-bottom-title">产品服务</span>
            <a
              href="https://www.haohuo.com"
              target="_blank"
              class="site-bottom-link"
              >好货</a
            >
            <a
              href="https://www.haohuo.com/goods/receiving"
              target="_blank"
              class="site-bottom-link"
              >接单广场</a
            >
            <a
              href="https://www.haohuo.com/goods/list"
              target="_blank"
              class="site-bottom-link"
              >达人选品库</a
            >
          </div>
        </div>
      </div>
      <div class="flex-column margin-right-20 site-top-item">
        <img
          src="https://xl.linkstars.com/asset/img/xingluo-components/xingluoguandian.png"
        />
        <span>二维码</span>
      </div>
      <div class="flex-column site-top-item">
        <img
          src="https://xl.linkstars.com/asset/img/xingluo-components/xingluoguandian.png"
        />
        <span>二维码</span>
      </div>
    </div>
    <div class="page-bottom-links">
      <div>@CopyRight 2019-2020 星罗www.linkstars.com</div>
      |
      <div>@CopyRight 2019-2020 星罗www.linkstars.com</div>
      |
      <div>鲁网文〔2020〕3486-062号</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Sitefooter',
  data() {
    return {}
  },
}
</script>

<style scoped>
.site-footer {
  /* padding: 20px 0; */
  background-color: #1f232b;
  color: #999;
}
.page-bottom-top {
  width: 1200px;
  justify-content: space-between;
  padding: 35px 0 25px;
}
.page-bottom-links {
  background: #191c23;
  height: 50px;
  width: 100%;
  line-height: 50px;
  text-align: center;
}
.page-bottom-links div {
  display: inline-block;
  font-size: 14px;
  text-decoration: none;
  color: #999;
}
.site-top-item img {
  width: 80px;
  margin-bottom: 10px;
}
.site-top-logo img {
  width: 144px;
  height: 74px;
  margin-top: 26px;
}
.site-bottom-fa {
  margin-left: 147px;
  display: flex;
}
.site-bottom:last-child {
  margin-left: 96px;
}
.site-bottom-title {
  margin-right: 20px;
  font-size: 16px;
  color: #fff;
}
.site-bottom-link {
  display: block;
  margin-top: 8px;
  text-decoration: none;
  font-size: 14px;
  color: #999;
}
</style>
