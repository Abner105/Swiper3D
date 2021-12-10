<template>
  <div class="banner-box">
    <div class="wrapper">
      <div class="slide">
        <img src="../assets/img/1.jpg" alt="" />
        <div class="mark activate"></div>
        <p class="detail">
          <span>蒙奇·D·路飞</span>
          <span>身份：草帽海贼团船长</span>
          <span>梦想：找到ONE PIECE，成为海贼王</span>
        </p>
      </div>
    </div>
    <a href="javascript:;" class="left"></a>
    <a href="javascript:;" class="right"></a>
  </div>
</template>

<script>
export default {
  name: "Swiper3D",
};
</script>

<style scoped>
.banner-box {
  width: 100%;
  height: 100%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background-color: rgba(0, 0, 0,0.5);
}
.wrapper {
  width: 100%;
  height: 100%;
  position: relative;
}
.slide {
  width: 25%;
  height: 100%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  /* background-color: azure; */
}
img {
  height: 100%;
  width: 100%;
  vertical-align: bottom;
}
.mark {
  position: absolute;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
}
.activate,
.mark:hover {
  background-color: rgba(0, 0, 0, 0);
}
.detail {
  display: flex;
  flex-direction: column;
  /* padding: 10px 0px; */
  position: absolute;
  bottom: 0;
  color: #fff;
  background-color: rgba(0, 0, 0, 0.5);
  max-height: 0px;
  overflow: hidden;
  transition: 0.2s;
  font-size: 14px;
  width: 100%;
}
.detail span{
  margin: 2px 10px;
}
.slide:hover .detail {
  max-height: 100%;
  padding: 5px 0px;
}
a.left {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  left: 0px;
  z-index: 9;
  /* background-color: black; */
  width: 50px;
  height: 50px;
  background-image: url(../assets/img/left.png);
  background-size: contain;
}
a.right {
  position: absolute;
  top: 50%;
  right: 0px;
  transform: translateY(-50%);
  z-index: 9;
  width: 50px;
  height: 50px;
  background-image: url(../assets/img/right.png);
  background-size: contain;
}
</style>
