<template>
  <div class="main">
    <div class="main-container">
      <Carousel :data="state.data" />
    </div>
  </div>
</template>

<script setup lang="ts">
import Carousel from "./components/Carousel/Carousel.vue";
import { EachData } from "./components/Carousel/types/Carousel";
import { reactive } from "vue";

const state = reactive({
  data: [
    {
      id: "lsfjlsfl",
      path: "/",
      url: "https://img2.baidu.com/it/u=3226783590,4049882211&fm=253&app=138&size=w931&n=0&f=JPEG&fmt=auto?sec=1677949200&t=f4fd94128db3166f599f9cab9dae5835",
    },
    {
      id: "lsf23esdjlsfl",
      path: "/",
      url: "https://img1.baidu.com/it/u=1247680594,3044752038&fm=253&app=138&size=w931&n=0&f=JPEG&fmt=auto?sec=1677949200&t=9bdd1bc12cee9d54cfa787e584bd078e",
    },
    {
      id: "lsf23esdjlsflmm",
      path: "/",
      url: "https://img1.baidu.com/it/u=2785121292,3860608278&fm=253&fmt=auto&app=138&f=JPEG?w=800&h=500",
    },
    {
      id: "lsf2sdjlsflmm",
      path: "/",
      url: "https://img1.baidu.com/it/u=4074323348,2604259187&fm=253&fmt=auto&app=138&f=JPEG?w=500&h=313",
    },
  ] as EachData[],
});
</script>

<style scoped lang="less">
.main {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}
.main-container {
  width: 700px;
  height: 500px;
  border: 1px solid #000;
}
</style>
