<script setup>
import linkedIn from "@/icons/icon-linked-in.svg";
import github from "@/icons/icon-github.svg";
import spotify from "@/icons/icon-spotify.svg";
const socialLinks = {
  github: {
    icon: github,
    link: "https://github.com/Ephalys",
  },
  linkedIn: {
    icon: linkedIn,
    link: "https://www.linkedin.com/in/leon-tran-van/",
  },
  spotify: {
    icon: spotify,
    link: "https://open.spotify.com/user/ephalys?si=UhyBFbz4S7qeLkMAkjliDg",
  },
};
</script>

<template>
  <div class="flex gap-10 items-center">
    <a
      v-for="(socialLink, index) in socialLinks"
      :key="index"
      :href="socialLink.link"
    >
      <img :src="socialLink.icon" alt="icon" width="18" height="18" />
    </a>
  </div>
</template>
