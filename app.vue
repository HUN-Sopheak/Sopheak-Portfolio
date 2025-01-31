<script setup lang="ts">
useHead({
  title: "Sopheak HUN - Portfolio | Web Developer",
  htmlAttrs: {
    lang: "en",
  },
  link: [{ rel: "icon", type: "image/png", href: "/favicon-16.png" }],
});

useSeoMeta({
  description:
    "Hi! I'm Sopheak HUN, a passionate Web Developer specializing in creating modern, responsive, and user-friendly websites.",
  author: "Sopheak HUN",
  ogTitle: "Sopheak HUN - Portfolio | Web Developer",
  ogDescription:
    "Hi! I'm Sopheak HUN, a passionate Web Developer specializing in creating modern, responsive, and user-friendly websites.",
  ogImage: "https://sopheak-hun.vercel.app/hero.jpg",
  ogUrl: "https://sopheak-hun.vercel.app/",
  ogType: "website",
  twitterCard: "summary_large_image",
  twitterTitle: "Sopheak HUN - Portfolio | Web Developer",
  twitterDescription:
    "Hi! I'm Sopheak HUN, a passionate Web Developer specializing in creating modern, responsive, and user-friendly websites.",
  twitterImage: "https://sopheak-hun.vercel.app/hero.jpg",
});
</script>

<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>
