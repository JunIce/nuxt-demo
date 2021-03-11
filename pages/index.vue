<template>
  <div class="index">
    <site-header :bg-visible="headerVisible" />
    <div class="top-banner">
      <div class="top-content">
        <div class="top-title">大海航行靠舵手<br />电商带货找星罗</div>
        <div class="top-desc">以技术驱动的商品与媒体匹配的全链路服务平台</div>
      </div>
    </div>
    <div class="section-second">
      <a href="/" class="card-item">
        <div class="card-item-title">电商带货平台</div>
        <div class="card-item-desc">
          星罗旗下好货网站<br />工具型平台实现货与流量的精准高效匹配
        </div>
        <img src="/images/card_item_img.png" class="card-item-imgl" />
        <div class="card-item-btn">
          查看详情<span class="card-item-btn-san"></span>
        </div>
      </a>
      <a href="/" class="card-item">
        <div class="card-item-title">电商带货平台</div>
        <div class="card-item-desc">
          星罗旗下好货网站<br />工具型平台实现货与流量的精准高效匹配
        </div>
        <img src="/images/card_item_img.png" class="card-item-imgl" />
        <div class="card-item-btn">
          查看详情<span class="card-item-btn-san"></span>
        </div>
      </a>
    </div>

    <div class="platform">
      <div class="platform-box">
        <div class="platform-title">
          <img
            src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAqCAYAAADI3bkcAAAAAXNSR0IArs4c6QAAA0BJREFUWAnVmMtvDVEcx3uFEJXShYZIhJAQsZA0dIN0YaGeG7rrohuxExt7C3+BtcSuiU09otUEifcGCSshiAU2RCQtqtrrc657budxHt+ZSzN+ybcz5/f4nu+c+c250+no+M+sViW99Xp9M3oGQR/4BB6DC7Va7SfHahlih8B3kLU3OLZXSi2C9mZVZsavGXdXRjRiHmUEuoanKyEYZVtd6hy+m0bwogqoPiJqaGiVBHO1u8El8AV8BHfBgDhRLO1oLKEZfy/lIewkmAEuOy+ReJIgXA1mXcQO37CHZt5N0RbgE2s5h+Yrip1BMGxJIkdzUT1RdpJGIkQm/CBK5EmgdlTg1+YgaxmYEgjN1S/1aPK6C/AbCWcsUeih20fScpsYOE7z0zkdiPtCKr+pv2pJQoLV7eatJSt4VPlfsSAvLLdTMLfAvBQdskmR43gkngs3+Q/nAm5Ha3VN2CkY/06w1iQIliIU8k3KLrBGzL2SzPMJVjfzz5CV2SXUdjD8DxXBKuF1+ms2SSiel+bPrTD9tZFJ1ffPwu3QLn9OMGLVqzdb2YS4osk0td2c/C7BKuFt2mEyqUQ8VxfEyZ8SzO1axaR7xInLtEPb/CnBCD0AFguC6+RcE/KyKW3zZwWrt+sp7aC9n6Ylq+32xMffEkw7LIFbfSlPbeZpTe5Rk3+/O5rzetutJZiSftCVK3U7vITu9Ia3n79t8ycFq+3wjtv1LCDMF/or/GUEl3nYzEWogoN3ryGY/toB4Xrf0mT8Zfq3CH9cMIIOZkT5hl8J3PEFA351daP8tiXMRzjFbtC/M0piJkcVHOW3grszE/iGwdvlKqLd1uHvdcUcvmi7WcGpd04HkXF9A2OeWMitru4vSLT/XliFDWAShOxcSJUvBuF4iDQRu+XjcPopPAbmEgTJ03sMupyFASc1K8CPJFHg/FSAyh2CrBdMAPs94iXnZ4H52S5s1A0A1cw/DuWNWTrLV/+phOOEqPa5Opd96HL5bF9TOWdxh/KqalgL7z7FpQgVrO4mYYXNp65tAt3CpCDGfFcO2cWFUSLOgtJOcN+jeAz/SpGqkWY+Sf1zQ5SZZxAcB+aL0gdwGYzwrMxxlO03x571hvNQYp0AAAAASUVORK5CYII="
            class="platform-title-icon"
          />
          多平台实力资质认证
          <img
            src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAqCAYAAADI3bkcAAAAAXNSR0IArs4c6QAAAxZJREFUWAnVmNuLTlEYxmePUQ6NqKGUGxGaUlIuHKKQyKmGciVx70+QK3In/AHcKBdKDCHnC4e5kJJyQWkak1AupkHEfH5r+g5rr2+9a7/v3n31WfW013t63mfPeme3v93T85+trIzeWq22kbohsAx8AreyLLvJtbsWQmeAsyC2HuLs7yrFCDoRU+r5rnWNYEQNgAlPnLRd20nRvQbyA+Rqjny3gdOcahG8T8lu4VRSttJU5Jz9XEq2tsqSu/FkNBGkzxHwAEyCUXAVDCZK4iGKhoB2uUedaUHsnj6XhAZ/8B+yEkpkYY83JuJ6MiTHQqLA/o69SsVNYi/4GhBI5mkVqZdU5x+TCD3/NLdmhjfAP+D1SG1vpIJCzPEvEWK+e4szNIL3+1WJ/WdiI4m4FNLyTzgCjWDt42yY94mapCrh1/J/KBTM/KwkaUWimR8yj4OR/3ahYBK0d/+D3Pu+euXezF80Etr5usc4/FSK9NPM/KJgjmshzOt99sS+zDi4J4+ZXxQMmXuJScUb+qfYlHl531OGPyVIO18jjMOXhnrDtRR/VDDjMIvGO5TNryvzmmlV+KOCYd4G3BuaZpnnF9LS/JJg7XG9Zxzeau4qyCnN3yaY43K/pPcGDSTT/Netyt8mGGXrwGJJYeA3z29V/phg7XF9o/nT4AY0ZiX+KoLdx5O/GoVBjlZwlD8nmPlaCvnqoIFklpnfyvw5wSjT3v0vcu9Id5LwV+YvK/gR4zCZECaFtN8sRP6mYMZhPl02S50Cv3kc6vXLAx7JFPmbgqncBfokhsA/HNhac4EyUeT3BWvfTV8yDh+VjcO0Z6EjYr9I8U8LZhxmUrgzUhxziccVSw58FwM7Zp6MOXM+BG8H2rUmV2w0aHIu0ei8ig6CMwkSPzSqIixIgvAgeA1+gynwHBwuKGuFSb4MNOtCq6r6joYZmGNhajwVGtei2irz28bNP5f7juF+catX4ylxV1ExRs5jRV7nUziWeeAdSK2jnVdi6IDSQTAuKD6FPzPQdSw1JwJRs+l0HGwCi8ArcIVZe8K1K9Y/zEAEi2009vQAAAAASUVORK5CYII="
            class="platform-title-icon"
          />
        </div>
        <div class="platform-bottom">
          <div class="platform-bottom-li platform-d">
            抖音电商首批品牌服务商&nbsp;&nbsp;&nbsp;&nbsp;
            <img
              src="~assets/images/platform_icon.png"
              class="platform-bottom-img"
            />
          </div>
          <div class="platform-bottom-li platform-t">
            <img
              src="~assets/images/platform_icon.png"
              class="platform-bottom-img"
            />
            &nbsp;&nbsp;&nbsp;&nbsp;淘宝联盟优秀招商服务商
          </div>
          <div class="platform-bottom-li platform-ju">
            巨量引擎“百大计划”服务商&nbsp;&nbsp;&nbsp;&nbsp;
            <img
              src="~assets/images/platform_icon.png"
              class="platform-bottom-img"
            />
          </div>
          <div class="platform-bottom-li platform-jd">
            <img
              src="~assets/images/platform_icon.png"
              class="platform-bottom-img"
            />
            &nbsp;&nbsp;&nbsp;&nbsp;京东联盟官方招商服务商
          </div>
          <div class="platform-bottom-li platform-k">
            快手好物联盟服务商&nbsp;&nbsp;&nbsp;&nbsp;
            <img
              src="~assets/images/platform_icon.png"
              class="platform-bottom-img"
            />
          </div>
          <div class="platform-bottom-li platform-w">
            <img
              src="~assets/images/platform_icon.png"
              class="platform-bottom-img"
            />
            &nbsp;&nbsp;&nbsp;&nbsp;唯品会官方内容服务商
          </div>
        </div>
      </div>
    </div>

    <div class="brand">
      <div class="brand-title">
        <img
          src="~assets/images/brand_icon_left.png"
          class="platform-title-icon"
        />
        合作品牌
        <img
          src="~assets/images/brand_icon_right.png"
          class="platform-title-icon"
        />
      </div>
      <div class="brand-box">
        <div class="brand-box-t">
          <div class="brand-li">
            <img src="/images/brand_logo.png" class="bw146" />
          </div>
          <div class="brand-li">
            <img src="/images/brand_logo.png" class="bw146" />
          </div>
          <div class="brand-li">
            <img src="/images/brand_logo.png" class="bw146" />
          </div>
          <div class="brand-li">
            <img src="/images/brand_logo.png" class="bw146" />
          </div>
          <div class="brand-li">
            <img src="/images/brand_logo.png" class="bw146" />
          </div>
        </div>
        <div class="brand-box-t">
          <div class="brand-li">
            <img src="/images/brand_logo.png" class="bw146" />
          </div>
          <div class="brand-li">
            <img src="/images/brand_logo.png" class="bw146" />
          </div>
          <div class="brand-li">
            <img src="/images/brand_logo.png" class="bw146" />
          </div>
          <div class="brand-li">
            <img src="/images/brand_logo.png" class="bw146" />
          </div>
          <div class="brand-li">
            <img src="/images/brand_logo.png" class="bw146" />
          </div>
        </div>
      </div>
    </div>
    <site-footer />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import SiteHeader from '@/components/site-header.vue'
import SiteFooter from '@/components/site-footer.vue'

export default Vue.extend({
  layout: 'default',
  components: {
    SiteHeader,
    SiteFooter,
  },
  data() {
    return {
      headerVisible: false,
    }
  },
  mounted() {
    window.addEventListener('scroll', this.onScroll, false)
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.onScroll)
  },
  methods: {
    onScroll() {
      const scrollTop = document.documentElement.scrollTop
      if (scrollTop < 90) this.headerVisible = false
      if (!this.headerVisible && scrollTop > 90) {
        this.headerVisible = true
      }
    },
  },
})
</script>

<style scoped>
.top-banner {
  display: flex;
  justify-content: center;
  width: 100%;
  height: 461px;
  background-image: url('~assets/images/home_bg.jpg');
}
.top-content {
  background: rgba(85, 105, 162, 0.28);
  width: 100%;
  height: 100%;
  text-align: center;
}
.top-title {
  height: 192px;
  margin-top: 117px;
  line-height: 96px;
  font-weight: 700;
  font-size: 80px;
  color: #fff;
}
.top-desc {
  background: hsla(0, 0%, 100%, 0.15);
  display: inline-block;
  width: 547px;
  margin-top: 33px;
  font-size: 24px;
  color: #fff;
  border: 1px solid #fff;
  border-radius: 26px;
}

.section-second {
  background: #fff;
  display: flex;
  justify-content: center;
  margin-top: 53px;
  margin-bottom: 53px;
}

.card-item {
  width: 582px;
  height: 495px;
  text-align: center;
  text-decoration: none;
  border-radius: 12px;
  cursor: pointer;
}
.card-item:hover {
  -webkit-transform: scale(1.1);
  transform: scale(1.1);
  box-shadow: 2px 1px 15px 1px hsla(0, 0%, 90.2%, 0.5);
}
.card-item-title {
  height: 72px;
  margin-top: 20px;
  line-height: 72px;
  font-weight: 700;
  font-size: 30px;
  color: #333;
}
.card-item-desc {
  line-height: 24px;
  font-size: 14px;
  color: #333;
}
.card-item-imgl {
  margin-top: 40px;
  width: 385px;
}
.card-item-btn {
  background: rgba(103, 118, 249, 0.9);
  display: none;
  justify-content: center;
  align-items: center;
  width: 113px;
  height: 36px;
  margin: 20px auto 0;
  line-height: 36px;
  font-size: 14px;
  color: #fff;
  box-shadow: 0 3px 7px 0 hsla(0, 6%, 67.5%, 0.5);
  border-radius: 26.5px;
  cursor: pointer;
}
.card-item-btn-san {
  width: 0;
  height: 0;
  margin-left: 10px;
  margin-right: -5px;
  border: 5px solid transparent;
  border-left-color: #fff;
}
.card-item:hover .card-item-btn {
  display: flex;
}

.platform {
  background-image: url('~assets/images/platform_bg.jpg');
  background-size: cover;
  height: 556px;
}
.platform-box {
  background: rgba(14, 27, 65, 0.25);
  width: 100%;
  height: 100%;
  padding-top: 33px;
  text-align: center;
}
.platform-title {
  height: 72px;
  font-weight: 700;
  font-size: 30px;
  color: #fff;
}

.platform-bottom {
  background: url('~assets/images/platform_bg_center.png') no-repeat 50%;
  background-size: 145px 175px;
  position: relative;
  width: 353px;
  height: 353px;
  margin: 35px auto 0;
  border: 1px solid rgba(194, 179, 239, 0.39);
  border-radius: 100%;
}

.platform-bottom-li {
  position: absolute;
  display: flex;
  align-items: center;
  font-size: 18px;
  color: #fff;
}
.platform-bottom-img {
  width: 75px;
  height: 75px;
}
.platform-d {
  top: 0;
  left: -200px;
}
.platform-t {
  top: 0;
  right: -200px;
}
.platform-ju {
  top: 139px;
  left: -290px;
}
.platform-jd {
  top: 139px;
  right: -268px;
}
.platform-k {
  top: 277px;
  left: -162px;
}
.platform-w {
  top: 277px;
  right: -180px;
}

.brand {
  margin-top: 43px;
  margin-bottom: 52px;
  font-size: 30px;
  text-align: center;
  color: #333;
}
.brand-title {
  font-weight: 700;
  height: 72px;
  line-height: 72px;
}
.platform-title-icon {
  width: 22px;
  height: 21px;
  margin-left: 4px;
}
.platform-title-icon:first-child {
  margin: 0 4px 0 0;
}
.brand-box {
  width: 1200px;
  margin: 25px auto 0;
}
.brand-box-t {
  display: flex;
  border-top: 1px solid hsla(0, 0%, 60%, 0.2);
}
.brand-box-t:last-child {
  border-bottom: 1px solid hsla(0, 0%, 60%, 0.2);
}
.brand-li {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 241px;
  height: 114px;
  border-left: 1px solid hsla(0, 0%, 60%, 0.2);
}
.brand-li:last-child {
  border-right: 1px solid hsla(0, 0%, 60%, 0.2);
}
.bw146 {
  width: 146px;
}
</style>
