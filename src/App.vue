<script setup>
import { ref } from "vue";
import Sidebar from "./layouts/Sidebar.vue";
import RightBar from "./layouts/RightBar.vue";
import MainSection from "./components/main-section/index.vue";

const verb = ref(null);
const conjugation = ref(null);
</script>

<template>
  <div
    class="container w-full flex flex-wrap justify-between mx-auto px-2 pt-8 lg:pt-16 mt-16"
  >
    <Sidebar @set="(e) => (verb = e)" />
    <MainSection :verb="verb" :conjugation="conjugation" />
    <RightBar @set="(e) => (conjugation = e)" />
  </div>
</template>

<style>
@import "./assets/base.css";

#app {
}
</style>
