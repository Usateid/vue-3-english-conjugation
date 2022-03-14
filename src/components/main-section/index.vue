<template>
  <div
    class="w-full lg:w-4/6 lg:px-6 text-xl text-center text-gray-800 leading-normal"
  >
    <p>Verb selected {{ verb }}</p>
    <p>conjugation selected {{ conjugation }}</p>
  </div>
</template>

<script setup>
"main-section";
defineProps({
  verb: {
    type: String,
    default: null,
  },
  conjugation: {
    type: String,
    default: null,
  },
});
</script>

<style lang="scss" scoped></style>
