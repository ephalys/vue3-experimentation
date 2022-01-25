<script setup>
import HomeText from "@/components/HomeText.vue";
import Socials from "@/components/Socials.vue";
import imageOfMe from "@/images/leon-tran-van.webp";
import signature from "@/images/signature.svg";
</script>

<template>
  <img :src="signature" alt="signature" class="mb-6 md:mb-12" height="12" />
  <HomeText class="order-1 md:w-1/2" />
  <div
    class="
      md:flex
      md:flex-col
      md:justify-center
      md:fixed
      md:right-8
      md:inset-y-16
      md:w-5/12
    "
  >
    <img :src="imageOfMe" alt="Image of me" class="w-full" />
    <Socials class="mt-6" />
  </div>
</template>
