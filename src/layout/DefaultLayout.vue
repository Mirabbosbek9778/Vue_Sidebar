<script setup>
import SideBar from "../components/Sidebar.vue";
</script>

<template>
  <div>
    <div class="flex">
      <SideBar class="w-[280px]" />
      <slot />
    </div>
  </div>
</template>

<style scoped></style>
