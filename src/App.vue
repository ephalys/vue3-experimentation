<script setup>
import { ref } from "vue";

let counter = ref(0);

setInterval(() => {
  counter.value++;
}, 1000);
</script>

<template>
  <main class="flex flex-col px-8 py-16 md:items-start">
    <router-view />
  </main>
</template>
