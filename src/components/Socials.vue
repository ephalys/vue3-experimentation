<script setup>
import linkedIn from "@/icons/icon-linkedin.svg";
import github from "@/icons/icon-github.svg";
import spotify from "@/icons/icon-spotify.svg";
import email from "@/icons/icon-mail.svg";
const socialLinks = {
  github: {
    icon: github,
    link: "https://github.com/Ephalys",
  },
  linkedIn: {
    icon: linkedIn,
    link: "https://www.linkedin.com/in/leon-tran-van/",
  },
  email: {
    icon: email,
    link: "mailto:nvnrtnl@gmail.com",
  },
  spotify: {
    icon: spotify,
    link: "https://open.spotify.com/user/ephalys?si=UhyBFbz4S7qeLkMAkjliDg",
  },
};
</script>

<template>
  <div class="flex gap-10 items-center justify-center">
    <a
      v-for="(socialLink, index) in socialLinks"
      :key="index"
      :href="socialLink.link"
      target="_blank"
    >
      <img
        :src="socialLink.icon"
        class="h-5 transition duration-300 hover:translate-y-[-5px]"
      />
    </a>
  </div>
</template>
