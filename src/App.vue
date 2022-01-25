<script setup>
import { ref } from 'vue'

let counter = ref(0)

setInterval(() => {
  counter.value++
}, 1000)
</script>

<template>
    <main class="px-8 py-16">
      <router-view />
    </main>
</template>
