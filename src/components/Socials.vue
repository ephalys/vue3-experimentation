<script setup>
import linkedIn from "@/icons/icon-linked-in.svg?component";
import github from "@/icons/icon-github.svg?component";
import spotify from "@/icons/icon-spotify.svg?component";
import email from "@/icons/icon-email.svg?component";
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
      <component
        :is="socialLink.icon"
        class="
          transition
          duration-300
          hover:fill-pink-400 hover:translate-y-[-5px]
        "
      />
    </a>
  </div>
</template>
