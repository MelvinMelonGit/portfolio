<script setup>
import { ref } from "vue";

const list = ref([1, 2, 3]);
</script>

<template>
  <li v-for="item of list">
    <a href="#">{{ item }}</a>
  </li>
</template>
