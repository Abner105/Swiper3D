<template>
  <div id="app">
    <swiper-3-d></swiper-3-d>
  </div>
</template>

<script>
import Swiper3D from "./components/Swiper3D.vue";

export default {
  name: "App",
  components: {
    Swiper3D,
  },
};
</script>

<style>
*{
  margin: 0;
  padding: 0;
}
#app {
  /* background-color: rgb(255, 213, 177); */
  background-image: url(./assets/img/hzw.jpg);
  position: relative;
  width: 1050px;
  height: 400px;
  /* background-color: aquamarine; */
  margin: 0 auto;
}
</style>
