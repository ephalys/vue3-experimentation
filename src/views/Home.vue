<script setup>
import HomeText from "@/components/HomeText.vue";
import Socials from "@/components/Socials.vue";
import imageOfMe from "@/images/leon-tran-van.webp";
import Signature from "@/components/Signature.vue";
</script>

<template>
  <Signature class="mx-auto mb-12 md:mx-0 signature" />
  <HomeText class="md:w-1/2" />
  <div
    class="
      mt-12
      md:flex
      md:flex-col
      md:justify-center
      md:fixed
      md:right-8
      md:inset-y-16
      md:w-5/12
      md:mt-0
    "
  >
    <img :src="imageOfMe" alt="Image of me" class="w-full" />
    <Socials class="mt-6" />
  </div>
</template>