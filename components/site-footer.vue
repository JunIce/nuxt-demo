<template>
  <div class="site-footer flex-column">
    <div class="flex-row page-bottom-top">
      <div class="site-top-logo">
        <img
          src="https://xl.linkstars.com/asset/img/xingluo-components/xingluo-components-page-bottom-logo.png"
        />
      </div>
      <div></div>
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
  height: 50px;
  line-height: 50px;
  background-color: #191c23;
  display: flex;
  justify-content: center;
}
.site-top-item img {
  width: 80px;
  margin-bottom: 10px;
}
.site-top-logo img {
  width: 16re0px;
}
</style>
