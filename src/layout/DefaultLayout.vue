<script setup>
import SideBar from "../components/Sidebar.vue";
import Card from "../components/genericCard/Card.vue";
import Filter from "../components/Filter.vue";
</script>

<template>
  <div class="flex w-full">
    <div class="flex border-spacing-1">
      <SideBar />
      <slot />
    </div>
    <div class="flex flex-col w-full pl-[46px] gap-5">
      <Filter />
      <Card class="w-full" />
      <Card />
      <Card />
      <Card />
    </div>
  </div>
</template>

<style scoped></style>
