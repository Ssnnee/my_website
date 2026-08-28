<script setup>
useHead({
  meta: [
    { name: 'viewport', content: 'width=device-width, initial-scale=1' }
  ],
  link: [
    { rel: 'icon', href: '/favicon.ico' }
  ],
  htmlAttrs: {
    lang: 'en'
  }
})

const title = 'Samuel Nandi'
const description = "Samuel Nandi's personal website and portfolio showcasing my work, projects, and skills"

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
  ogImage: 'https://ui.nuxt.com/assets/templates/nuxt/starter-light.png',
  twitterCard: 'summary_large_image'
})
</script>

<template>
  <div class ="mx-auto w-[min(900px,calc(100%-40px))] text-(--fg) max-[600px]:w-[min(calc(100%-28px),900px)]">
    <UApp>
      <NavLink class="w-auto text-accent" />
      <UMain>
        <NuxtPage />
      </UMain>
  </UApp>
</div>
</template>
