<script setup lang="ts">
useHead({
  title: 'Sopheak HUN-Portfolio',
  htmlAttrs: {
    lang: 'en',
  },
  meta: [
    { charset: 'UTF-8' },
    { name: "viewport", content:"width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0" },
    {
      name: 'description',
      content:
        '',
    },
    { name: 'author', content: 'Sopheak HUN' },
    { property: 'og:type', content: 'website' },
    { property: 'og:url', content: '/hero.jpg' },
    {
      property: 'og:title',
      content: 'Sopheak HUN Portfolio',
    },
    {
      property: 'og:image',
      content:
        '/hero.jpg',
    },
    {
      property: 'og:description',
      content:
        "Hi! I'm Sopheak HUN, Web Developer",
    },

    {
      property: 'twitter:card',
      content:
        '/hero.jpg',
    },
    {
      property: 'twitter:title',
      content: 'Sopheak HUN Portfolio',
    },
    {
      property: 'twitter:description',
      content:
        "Hi! I'm Sopheak HUN, Web Developer",
    },
  ],
  link: [{ rel: 'icon', type: 'image/png', href: '/favicon-16.png' }],
})
</script>

<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>
