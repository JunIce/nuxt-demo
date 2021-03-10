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
</style>
