<script setup>
import { computed, ref } from "vue";

const navList = computed(() => [
  {
    title: "Logo",
    path: "/Logo",
    icon: "/src/assets/icons/logo.svg",
  },
  {
    title: "home",
    path: "/home",
    icon: "",
  },
  {
    title: "home",
    path: "/home",
    icon: "/src/assets/icons/home.svg",
  },
  {
    title: "search",
    path: "/search",
    icon: "/src/assets/icons/search.svg",
  },
  {
    title: "menu",
    path: "/menu",
    icon: "/src/assets/icons/menu.svg",
  },
  {
    title: "tvIcon",
    path: "/tvIcon",
    icon: "/src/assets/icons/tvIcon.svg",
  },
  {
    title: "favouriteIcon",
    path: "/favourite",
    icon: "/src/assets/icons/favouriteIcon.svg",
  },
  {
    title: "profile",
    path: "/profile",
    icon: "",
  },
  {
    title: "notification",
    path: "/notification",
    icon: "",
  },
  {
    title: "settings",
    path: "/settings",
    icon: "",
  },
  {
    title: "settings",
    path: "/1",
    icon: "",
  },
  {
    title: "profile",
    path: "/profile",
    icon: "/src/assets/icons/profile.svg",
  },
  {
    title: "notification",
    path: "/notification",
    icon: "/src/assets/icons/notification.svg",
  },
  {
    title: "settings",
    path: "/settings",
    icon: "/src/assets/icons/settings.svg",
  },
]);
const activeNavIndex = ref(null);
</script>

<template>
  <div class="h-screen wrapper  py-10 ">
    <ul class="flex flex-col  mr-[140px]">
      <li
        v-for="(nav, index) in navList"
        :key="nav"
        class="flex flex-col items-center"
      >
        <router-link outer-link :to="nav.path">
          <div
            class="flex  gap-4 py-4 justify-start"
            @click="activeNavIndex = index"
            :class="{ 'active-nav': activeNavIndex === index }"
          >
            <img :src="nav.icon" alt="" />
          </div>
        </router-link>
      </li>
    </ul>
  </div>
</template>

<style scoped>
.wrapper {
  box-shadow: 0px 2px 1px -1px rgba(0, 0, 0, 0.2),
    0px 1px 1px 0px rgba(0, 0, 0, 0.14), 0px 1px 3px 0px rgba(0, 0, 0, 0.12);
}
.active-nav {
  background: rgba(33, 150, 243, 0.08);
  box-shadow: 0px 0px rgba(0, 0, 0, 0.25);
}
</style>
