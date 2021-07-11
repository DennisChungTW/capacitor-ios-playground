<template lang="pug">
main(
  class="xl:(container mx-auto) m-0 px-5 lg:px-10 py-10 flex flex-col items-center min-h-screen"
)
  h1(
    class="text-gray-700 text-4xl text-center font-black"
  ) Capacitor Playground
  hr.border-none.h-4.bg-yellow-300.min-w-72.mt-2.rounded-lg.flex-shrink-0
  span.text-gray-500 Try testing your capacitor app here

  div(
    class="w-[100%] lg:m-12 m-4 grid lg:grid-cols-3 sm:grid-cols-2 grid-cols-1"
    class="gap-4 md:gap-6 lg:gap-8"
  )
    FieldCard(title="Environment") 
      EnvironmentChunk(title="Capacitor")
        ToolTag CocoaPod
      EnvironmentChunk(title="VS Code")
        ToolTag Volar
        ToolTag WindiCSS
        ToolTag ESLint
        ToolTag Prettier
      EnvironmentChunk(title="Structure")
        ToolTag Vite
        ToolTag Vue3
        ToolTag WindiCSS
        ToolTag Pug(Jade)
        ToolTag SCSS

    FieldCard(title="Counter Example") 
      Counter
    FieldCard(title="Start form here")
      PlaceHolder
    FieldCard(title="Cap open browser")
      OpenLinkPanel
  div(aria-hidden class="flex-grow")
  footer(
    class="text-gray-600 mt-4"
  )
    | Dennis Chung @ 
    a(
      class="text-cool-gray-700 font-bold underline underline-gray-400"
      title="Hikari's github"
      href="https://github.com/hikariNTU"
      target="_blank"
      rel="noopener"
    ) Github
</template>

<script setup>
import Counter from "/@/components/Counter.vue";
import FieldCard from "/@/components/FieldCard.vue";
import EnvironmentChunk from "/@/components/EnvironmentChunk.vue";
import ToolTag from "/@/components/ToolTag.vue";
import PlaceHolder from "/@/components/PlaceHolder.vue";
import OpenLinkPanel from "./components/OpenLinkPanel.vue";
</script>
