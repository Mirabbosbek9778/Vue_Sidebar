<script setup>
import { ref } from "vue";

const show = ref(true);
</script>
<template>
  <div class="card">
    <div class="content">
      <h1>Новинки фильмов</h1>
      <div class="flex box">
        <transition name="el-fade-in" v-for="index in 4" :key="index">
          <div v-show="show" class="transition-box"></div>
        </transition>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  width: 100%;
  max-width: 1440px;
  margin: 0 auto;
  border-radius: 40px;
  background: rgba(255, 255, 255, 0.08);
  height: 312px;
  padding: 20px 0 0px 40px;
}

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
  margin-right: 20px;
}

h1 {
  color: #fff;
  text-align: center;
  font-family: SF Pro Display, sans-serif;
  font-size: 24px;
  font-style: normal;
  font-weight: 700;
  line-height: 100%;
  text-transform: uppercase;
  padding-top: 40px;
}
</style>
