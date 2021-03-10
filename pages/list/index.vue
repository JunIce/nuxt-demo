<template>
  <div class="index">
    <site-header />
    <div class="container">
      <h1>123</h1>
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
})
</script>

<style scoped>
.site-header {
  height: 70px;
  background-color: #251f44;
  display: flex;
  align-items: center;
  justify-content: center;
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

.site-header--menu-border {
  background: #5d33d7;
  width: 17px;
  height: 3px;
  margin: 0 auto;
  border-radius: 3px;
}
.container {
  min-width: 1200px;
  background-color: #f9f9f9;
}
</style>
