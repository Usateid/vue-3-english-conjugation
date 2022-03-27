<script setup>
import { ref } from "vue";
import verbs from "./components/verbs/index.vue";
import conjugations from "./components/conjugations/index.vue";
import MainSection from "./components/main-section/index.vue";

const verb = ref(null);
const conjugation = ref(null);
</script>

<template>
  <div class="container w-full flex flex-wrap justify-between mx-auto px-2 pt-8 lg:pt-16 mt-16">
    <verbs @set="(e) => (verb = e)" />
    <MainSection :verb="verb" :conjugation="conjugation" />
    <conjugations @set="(e) => (conjugation = e)" />
  </div>
</template>

<style>
@import "./assets/base.css";

#app {
}
</style>
