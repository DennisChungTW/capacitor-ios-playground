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
    FieldCard(title="Enviroment") 
      EnviromentChunk(title="Capacitor")
        ToolTag CocoaPod
      EnviromentChunk(title="VS Code")
        ToolTag Volar
        ToolTag WindiCSS
        ToolTag ESLint
        ToolTag Prettier
      EnviromentChunk(title="Structure")
        ToolTag Vite
        ToolTag Vue3
        ToolTag WindiCSS
        ToolTag Pug(Jade)
        ToolTag SCSS

    FieldCard(title="Counter Example") 
      Couter
    FieldCard(title="Start form here")
      PlaceHolder
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
import Couter from '/@/components/Couter.vue'
import FieldCard from '/@/components/FieldCard.vue'
import EnviromentChunk from '/@/components/EnviromentChunk.vue'
import ToolTag from '/@/components/ToolTag.vue';
import PlaceHolder from '/@/components/PlaceHolder.vue';
</script>
