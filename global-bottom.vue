<script setup>
import { useNav } from '@slidev/client'

const nav = useNav()
</script>

<template>
  <footer
      v-if="$nav.currentLayout !== 'cover'"
      class="page-number"
  >
    {{ $nav.currentPage }}
  </footer>
</template>

<style>
.page-number {
  position: fixed;
  bottom: 10px;
  right: 20px;
  color: #1a1a1a !important;
  font-size: 14px;
  font-family: monospace;
  z-index: 9999;
}
</style>
