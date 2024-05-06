<script setup>
import tailwindLogo from '../assets/tailwind.svg'
</script>

<template>
  <h1 class="flex flex-col sm:flex-row gap-4">
    <img class="not-prose h-16 w-min" :src="tailwindLogo" />
    <span>Hello Tailwind CSS!</span>
  </h1>
  
  <p class="lead clear-both">Typography should be easy</p>
  <p>
    Now I'm going to show you an example of an unordered list to make sure that
    looks good, too:
  </p>
  <ul>
    <li>So here is the first item in this list.</li>
    <li>In this example we're keeping the items short.</li>
    <li>Later, we'll use longer, more complex list items.</li>
  </ul>
  <p>And that's the end of this section.</p>
</template>
