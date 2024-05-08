<script setup>
import { ref } from "vue"
const inputHTML = ref('')
</script>
<template>
  <div class="flex">
  <div class="flex-none w-[20vw]">
    <div v-html="inputHTML"></div>
  </div>
  <div class="flex-1">
    <textarea class="text-black font-mono w-full h-[64vh]" @change="inputHTML = $event.target.value">
    </textarea>
  </div>
</div>
</template>
