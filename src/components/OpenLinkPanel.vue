<template lang="pug">
div(
  class="flex flex-grow justify-center items-center"
)
  a(
    href="https://hikarintu.github.io/sawano-translator/"
    title="sawano translator"
    class="border px-4 py-2 rounded-xl border-5 text-gray-700"
    @click.prevent="openCapacitorSite('https://hikarintu.github.io/sawano-translator/')"
  ) Open this link
</template>

<script setup>
import { Browser } from '@capacitor/browser';
const openCapacitorSite = async (url) => {
  await Browser.open({
    url,
  })
}
</script>