<script setup lang="ts">
import { computed } from 'vue'
import type { NavigationMenuItem } from '@nuxt/ui'

const route = useRoute()

const items = computed<NavigationMenuItem[]>(() => [{
      label: 'about',
      to: '#about',
  active: route.path.startsWith('#about')
}, {
  label: 'projects',
  to: '#projects',
  active: route.path.startsWith('#projects')
}, {
  label: 'contact',
  to: '#contact',
},
])
</script>

<template>
  <UHeader :ui="{ toggle: 'sm:hidden', container: 'px-0 sm:px-0 lg:px-0' }">
      <template #left>
        <NuxtLink to="/">
          <AppLogo class="" />
        </NuxtLink>
      </template>

    <template #right>
      <UNavigationMenu :items="items" class="hidden sm:flex" />
      <UColorModeButton />
    </template>

    <template #body>
      <UNavigationMenu :items="items" orientation="vertical" class="" />
    </template>

  </UHeader>
</template>


