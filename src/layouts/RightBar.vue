<template>
  <div class="w-full lg:w-1/6 lg:px-6 text-xl text-gray-800 leading-normal">
    <p class="text-base font-bold py-2 lg:pb-6 text-gray-700">English Verbs</p>
    <div
      class="w-full sticky inset-0 hidden h-64 lg:h-auto overflow-x-hidden overflow-y-auto lg:overflow-y-hidden lg:block mt-0 border border-gray-400 lg:border-transparent bg-white shadow lg:shadow-none lg:bg-transparent z-20"
      style="top: 5em"
      id="menu-content"
    >
      <ul class="list-reset">
        <li
          v-for="(item, i) in items"
          :key="`sidebar-element-${i}`"
          class="py-2 md:my-0"
        >
          <span
            class="block pl-4 align-middle text-gray-700 no-underline border-l-2 border-transparent lg:hover:border-red-500"
          >
            <span
              @click="$emit('set', item.value)"
              class="pb-1 md:pb-0 text-sm italic"
              >{{ item.value }}</span
            >
          </span>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
const items = [
  { value: "Present" },
  { value: "Preterite" },
  { value: "Present continuous" },
  { value: "Present perfect" },
  { value: "Future" },
  { value: "Past continous" },
  { value: "Past perfect" },
  { value: "Future continuous" },
  { value: "Present perfect continuous" },
  { value: "Past perfect continuous" },
  { value: "Future perfect continuous" },
  { value: "Imperative" },
  { value: "Participle Present" },
  { value: "Participle Past" },
  { value: "Infinitive" },
  { value: "Perfect Participle" },
];
</script>

<style lang="scss" scoped></style>
