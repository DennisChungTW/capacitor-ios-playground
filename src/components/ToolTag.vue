<template lang="pug">
li.tool-tag
  div.z-10.ml-4 
    slot
</template>

<style>
.tool-tag{
  @apply inline-flex bg-light-700 pr-5 py-2 m-1 ml-4 rounded-lg h-8 place-items-center;
  @apply text-gray-800 font-semibold;
  @apply before:content before:block before:h-5 before:w-5 before:bg-light-700;
  @apply before:absolute before:transform before:ml-[-7.5px] before:rotate-45;
  @apply before:rounded-bl-md;
}
</style>