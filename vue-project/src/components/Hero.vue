<script setup>
import { ref } from "vue";

const name = ref("Melvin");
const filled = ref("");

// setInterval(function () {
//   if (!filled.value) {
//     filled.value =
//       "bg-clip-text text-transparent bg-gradient-to-r from-pink-500 to-violet-500 border-b-4 border-indigo-500";
//   } else {
//     filled.value = "";
//   }
// }, 1500);
</script>

<template>
  <section class="flex items-center py-16">
    <div class="basis-3/4 mr-24">
      <h1 class="text-5xl font-semibold mb-8">
        Nice to meet you! <br />
        I'm
        <span :class="filled" class="border-b-4 border-pink-500">
          {{ name }}.
        </span>
      </h1>
      <p class="break-normal mb-10">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. In cursus turpis
        massa tincidunt dui ut ornare. Turpis egestas pretium aenean pharetra
        magna ac placerat vestibulum lectus.
      </p>
      <a href="#" class="border-b-2 border-pink-500">Contact Me</a>
    </div>
    <img src="https://picsum.photos/id/16/500" alt="the seas" class="grow" />
  </section>
</template>
