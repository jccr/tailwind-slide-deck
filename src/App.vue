<script setup>
import SlideLayout from './components/SlideLayout.vue'
import SlideControls from './components/SlideControls.vue'
</script>

<template>
  <SlideLayout>
    <RouterView />
  </SlideLayout>
  <SlideControls />
</template>
