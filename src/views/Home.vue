<script setup>
import signature from "@/images/signature.svg";
import HomeText from "@/components/HomeText.vue";
</script>

<template>
  <div class="flex flex-col gap-10 items-start">
    <img :src="signature" alt="signature" class="h-12" />
    <HomeText/>
  </div>
</template>
