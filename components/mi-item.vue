<template>
  <div class="item">
    <a class="item-img">
      <img
        src="//cdn.cnbj0.fds.api.mi-img.com/b2c-mimall-media/c06ee8f558c37f2bacd730070e276216.jpg?w=592&h=522"
      />
    </a>
    <div class="item-con">
      <a class="title">米家互联网洗烘一体机10kg</a>
      <p class="infor">烘干除菌率达99.9%</p>
      <p class="price" style="color: rgb(234, 98, 91)">
        <sup>¥</sup><span>1899</span><del><sup>¥</sup><span>2299</span></del>
      </p>
      <a href="" class="buy-btn">立即购买</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MiItem',
}
</script>

<style scoped>
.item {
  width: 300px;
  background: #fff;
}
.item-img {
  width: 100%;
  height: 260px;
  display: block;
  overflow: hidden;
}
.item-img img {
  display: block;
  width: 100%;
  height: 100%;
  background: #e6e6e6;
  transition: transform 0.6s ease-in-out;
  transform: scale(1) translateZ(0);
}
.item-img img:hover {
  transform: scale(1.05);
}

.item-con {
  text-align: center;
  padding-bottom: 10px;
}

.item-con .title {
  font-weight: 400;
  font-size: 20px;
  display: block;
  color: #242424;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  margin-top: 10px;
}

.item-con .infor {
  font-size: 14px;
  line-height: 18px;
  height: 18px;
  overflow: hidden;
  color: #666;
  margin: 0;
}

.item-con .price {
  font-size: 24px;
  margin-bottom: 0;
}

.item-con .price del {
  font-size: 14px;
  margin-left: 10px;
  display: inline-block;
  color: #666;
}

.buy-btn {
  background: #fd5452;
  border-radius: 2px;
  width: 124px;
  height: 40px;
  line-height: 40px;
  text-align: center;
  display: block;
  text-decoration: none;
  color: #fff;
  font-size: 14px;
  border: none;
  margin: 10px auto;
}
</style>
