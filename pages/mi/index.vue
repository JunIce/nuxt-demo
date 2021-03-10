<template>
  <div>
    <div class="section-title">
      <img
        src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/c7e22d96380a523b3c67d389da7afeba.jpg"
      />
    </div>
    <div class="container">
      <div class="list-container">
        <div
          v-for="(item, idx) in new Array(8)"
          :key="idx"
          class="list-container__item"
        >
          <activity-item />
        </div>
      </div>
    </div>

    <div class="section-title">
      <img
        src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/b1cb58d4f4586c0d34b630fe465d6245.jpg"
      />
    </div>
    <div class="container">
      <div class="list-container">
        <div
          v-for="(item, idx) in new Array(8)"
          :key="idx"
          class="list-container__item"
        >
          <activity-item />
        </div>
      </div>
    </div>

    <div class="section-title">
      <img
        src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/b1cb58d4f4586c0d34b630fe465d6245.jpg"
      />
    </div>
    <div class="container">
      <div class="list-container">
        <div
          v-for="(item, idx) in new Array(8)"
          :key="idx"
          class="list-container__item"
        >
          <activity-item />
        </div>
      </div>
    </div>

    <div class="section-title">
      <img
        src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/b1cb58d4f4586c0d34b630fe465d6245.jpg"
      />
    </div>
    <div class="container">
      <div class="list-container">
        <div
          v-for="(item, idx) in new Array(8)"
          :key="idx"
          class="list-container__item"
        >
          <activity-item />
        </div>
      </div>
    </div>

    <div class="section-title">
      <img
        src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/b1cb58d4f4586c0d34b630fe465d6245.jpg"
      />
    </div>
    <div class="container">
      <div class="list-container">
        <div
          v-for="(item, idx) in new Array(8)"
          :key="idx"
          class="list-container__item"
        >
          <activity-item />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ActivityItem from '~/components/mi-item'
export default {
  layout: 'xiaomi-activity',
  components: {
    ActivityItem,
  },
  data() {
    return {}
  },
}
</script>

<style scoped>
.container {
  background-color: #e1241e;
}
.list-container {
  margin: 0 auto;
  width: 1260px;
  display: flex;
  flex-wrap: wrap;
}
.list-container__item {
  width: 25%;
  margin-top: 16px;
}

.section-title {
  width: 100%;
  position: relative;
  height: 100px;
}
.section-title img {
  width: 100%;
  height: 100%;
}
</style>
