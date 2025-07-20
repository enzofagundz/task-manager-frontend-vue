<script setup lang="ts">
import { LayoutDefault, LayoutGuest } from '@/components'
</script>

<template>
  <LayoutGuest v-if="$route.meta.layout === 'guest'">
    <RouterView />
  </LayoutGuest>
  <LayoutDefault v-else>
    <RouterView />
  </LayoutDefault>
</template>
