<template lang="pug">
main(class="m-0 p-5 bg-gray-100 flex flex-col items-center justify-center h-screen")
  h1.text-gray-700.text-4xl Capacitor Playground
  hr.border-none.h-4.bg-yellow-300.w-72.mt-2.rounded-lg
  span Try testing your capacitor app here
    Hello
</template>

<script>
import { defineComponent } from "vue"
import Hello from '/@/components/Hello.vue'

export default defineComponent({
  components: {
    Hello
  },
  setup(){
    return {
      env: process.env.NODE_ENV,
    }
  }
});
</script>
