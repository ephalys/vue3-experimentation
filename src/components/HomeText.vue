<script setup>
const title =
  "Hi, I’m Léon Tran-Van. I’m currently working as a front-end developer at Hager, a leading supplier of solutions and services for electrical installations.";

const paragraphs = [
  "I began my career with an internship as fullstack developer at Classicat's. My objectives was to create a new site from scratch with an administration interface and increase traffic using good SEO practices.",
  "Then, I was full-stack developer at Subskill and for them I have worked on projects involving several fields, from luxury fashion brands to banks, from public services to health insurance, to major retail distributors and ecommerce.",
  "I'm always taking advantage of new technologies and current design trends in order to deliver the perfect product to my clients. That's why JAMstack and Figma take an important part in my workflow.",
  "In my spare time, I enjoy playing some video games, go play billiards, going to the gym and do motorcycle rides with friends."
]
</script>

<template>
    <h1 class="text-2xl font-bold">
      {{title}}
    </h1>
    <p v-for="(paragraph, index) in paragraphs" :key="index" class="text-base">
      {{paragraph}}
    </p>
</template>
