<script setup>
import Sidebar from "./layouts/Sidebar.vue";
import RightBar from "./layouts/RightBar.vue";
</script>

<template>
  <div
    class="container w-full flex flex-wrap justify-between mx-auto px-2 pt-8 lg:pt-16 mt-16"
  >
    <Sidebar />
    <RightBar />
  </div>
</template>

<style>
@import "./assets/base.css";

#app {
}
</style>
