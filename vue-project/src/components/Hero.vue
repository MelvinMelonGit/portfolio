<script setup>
import { ref } from "vue";

const name = ref("Melvin");
const filled = ref("");

// setInterval(function () {
//   if (!filled.value) {
//     filled.value =
//       "bg-clip-text text-transparent bg-gradient-to-r from-pink-500 to-violet-500";
//   } else {
//     filled.value = "";
//   }
// }, 1500);
</script>

<template>
  <h1 class="text-5xl font-semibold">
    Nice to meet you! <br />
    I'm
    <span :class="filled">
      {{ name }}
    </span>
  </h1>
</template>
