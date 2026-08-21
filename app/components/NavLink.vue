<script setup lang="ts">
  import type { NavigationMenuItem } from '@nuxt/ui'

  const items = ref<NavigationMenuItem[]>([
    {
      label: 'about',
      to: '#about',
    },
    {
      label: 'projects',
      to: '#projects'
    },
    {
      label: 'contact',
      to: '#contact'
    }
  ])
</script>

<template>
  <UNavigationMenu
    class="font-mono"
    :items="items"
    variant="link"
    :ui="{
      link: 'text-[#a3a3a3]'
    }"
  />
</template>
