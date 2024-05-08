<script setup>
import { ref } from 'vue'
import { Switch } from '@headlessui/vue'

const enabled = ref(false)
</script>

<template>
  <h1>Switch (Toggle)</h1>
  <div class="flex">
    <div class="ml-8 flex-none w-48">
      <div class="scale-125">
        <Switch
          v-model="enabled"
          :class="enabled ? 'bg-blue-600' : 'bg-gray-200'"
          class="relative inline-flex h-6 w-11 items-center rounded-full"
        >
          <span class="sr-only">Enable notifications</span>
          <span
            :class="enabled ? 'translate-x-6' : 'translate-x-1'"
            class="inline-block h-4 w-4 transform rounded-full bg-white transition"
          />
        </Switch>
      </div>
    </div>
    <div class="flex-1">
      <iframe
        class="w-full h-[75vh]"
        src="https://headlessui.com/v1/vue/switch#basic-example"
      />
    </div>
  </div>
</template>
