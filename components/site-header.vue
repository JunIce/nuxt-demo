<template>
  <div class="site-header" :class="{ black: bgVisible }">
    <div class="site-header--main">
      <div class="site-header--logo">
        <img
          src="https://xl.linkstars.com/asset/img/xingluo-components/xingluo-components-page-head-left-img.png"
        />
      </div>

      <div class="site-header--menu">
        <a class="site-header--menu-item">
          <nuxt-link to="/">
            <span>首页</span>
            <div class="site-header--menu-border"></div>
          </nuxt-link>
        </a>
        <a class="site-header--menu-item">
          <span>成功案例</span>
        </a>
        <a class="site-header--menu-item">
          <span>创作者服务</span>
        </a>
        <a class="site-header--menu-item">
          <nuxt-link to="/list">
            <span>商品总库</span>
            <div class="site-header--menu-border"></div>
          </nuxt-link>
        </a>
        <a class="site-header--menu-item">
          <span>开放平台</span>
        </a>
        <a class="site-header--menu-item">
          <span>合作项目</span>
        </a>
        <a class="site-header--menu-item">
          <span>帮助中心</span>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['bgVisible'],
  setup() {
    return {}
  },
}
</script>

<style scoped>
.site-header {
  background-color: transparent;
  display: flex;
  align-items: center;
  justify-content: center;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 70px;
  z-index: 10;
}
.black {
  background-color: #1f232b;
}
.site-header--main {
  width: 1200px;
  display: flex;
  color: #ffffff;
  font-size: 16px;
  justify-content: space-between;
}

.site-header--logo img {
  width: 90px;
}

.site-header--menu {
  display: flex;
  align-items: center;
}

.site-header--menu-item {
  font-size: 14px;
  color: #ffffff;
  margin-right: 20px;
  height: 40px;
  line-height: 40px;
}
.site-header--menu-item a {
  color: #fff;
}

.site-header--menu-border {
  background: #5d33d7;
  width: 17px;
  height: 3px;
  margin: 0 auto;
  border-radius: 3px;
}

.nuxt-link-exact-active {
  color: green;
}
</style>
