<template>
  <div class="border m-4 grid grid-cols-2 gap-2">
    <template v-for="type in tagList" :key="type">
      <label class="border">
        {{ type }}
        <input :type="type" />
      </label>
    </template>
  </div>
</template>

<script setup>
import { ref } from "vue"
const tagList = ref([
  "button",
  "checkbox",
  "color",
  "date",
  "datetime-local",
  "email",
  "file",
  "hidden",
  "image",
  "month",
  "number",
  "password",
  "radio",
  "range",
  "reset",
  "search",
  "submit",
  "tel",
  "text",
  "time",
  "url",
  "week",
])
</script>
