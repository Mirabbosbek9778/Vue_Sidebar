<script setup>
import { ref } from "vue";

const show = ref(true);
</script>
<template>
  <div class="wrapper border flex justify">
    <div class="flex flex-col items-center">
      <h1>Hовинки фильмов</h1>
      <div class="flex ">
        <transition name="el-fade-in-linear">
          <div v-show="show" class="transition-box"></div>
        </transition>
        <transition name="el-fade-in">
          <div v-show="show" class="transition-box"></div>
        </transition>
        <transition name="el-fade-in">
          <div v-show="show" class="transition-box"></div>
        </transition>
        <transition name="el-fade-in">
          <div v-show="show" class="transition-box"></div>
        </transition>
      </div>
    </div>
  </div>
</template>

<style scoped>
.transition-box {
  margin-bottom: 10px;
  border-radius: 4px;
  background: #202020;
  text-align: center;
  color: #fff;
  box-sizing: border-box;
  width: 316px;
  height: 178px;
  justify-content: center;
  align-items: center;
  border-radius: 16px;
  margin-top: 30px;
}
.wrapper {
  width: 100%;
  gap: 20px;
  border-radius: 40px;
  background: rgba(255, 255, 255, 0.08);
  height: 312px;
}
h1 {
  color: #fff;
  text-align: center;
  font-family: SF Pro Display, sans-serif;
  font-size: 24px;
  font-style: normal;
  font-weight: 700;
  line-height: 100%; /* 24px */
  text-transform: uppercase;
  padding-top: 40px;
}
</style>
