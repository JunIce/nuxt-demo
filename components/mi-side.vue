<template>
  <div class="mi-side">
    <a class="mi-side__item">
      <div>

      </div>
      <span>手机APP</span>
    </a>
  </div>
</template>

<script>
export default {
  name: 'MiSide',
  data() {
    return {}
  },
}
</script>

<style scoped>
.mi-side {
  position: absolute;
  right: 0;
  bottom: 100px;
}
.mi-side__item {
  position: relative;
  display: block;
  width: 82px;
  height: 90px;
  margin-top: -1px;
  background-color: #fff;
  border: 1px solid #f5f5f5;
  text-align: center;
}
</style>
