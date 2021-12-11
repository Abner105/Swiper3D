<template>
  <div id="app">
    <swiper-3-d :source="source"></swiper-3-d>
  </div>
</template>

<script>
import Swiper3D from "./components/Swiper3D.vue";

// 准备传入子组件中的数据
const source = [
  {
    id:1,
    pic:require("./assets/img/1.jpg"),
    descript:{
      name:"蒙奇·D·路飞",
      identity:"船长",
      dream:"梦想成为“海贼王”，以此为目标在大海上航行。"
    }
  },
    {
    id:2,
    pic:require("./assets/img/2.jpg"),
    descript:{
      name:"乌索普",
      identity:"狙击手",
      dream:"梦想“成为勇敢的海上战士”，以此为目标在大海上航行。"
    }
  },
    {
    id:3,
    pic:require("./assets/img/3.jpg"),
    descript:{
      name:"罗罗诺亚·索隆",
      identity:"三刀流剑士",
      dream:"梦想成为“世界第一大剑豪”，以此为目标在大海上航行。"
    }
  },
    {
    id:4,
    pic:require("./assets/img/4.jpg"),
    descript:{
      name:"山治",
      identity:"厨师",
      dream:"梦想“找到传说中的海域·All Blue”，以此为目标在大海上航行。"
    }
  },
    {
    id:5,
    pic:require("./assets/img/5.jpg"),
    descript:{
      name:"弗兰奇",
      identity:"船匠",
      dream:"梦想“乘坐自己制作的梦想之船绕伟大航路一周”，以此为目标在大海上航行。"
    }
  },
    {
    id:6,
    pic:require("./assets/img/6.jpg"),
    descript:{
      name:"娜美",
      identity:"航海士",
      dream:" 梦想绘制“全世界的地图”，以此为目标在大海上航行。"
    }
  },
]

export default {
  name: "App",
  components: {
    Swiper3D,
  },
  setup(){
    return{
      source
    }
  }
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
