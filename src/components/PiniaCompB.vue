<script setup lang="ts">
import { useCounterStore } from '@/stores/counter'

const counterStore = useCounterStore()
</script>

<template>
  <div class="grid">
    <code>PiniaCompB.vue</code>
    <pre>{{ counterStore }}</pre>
    <h1 class="text-4xl">{{ counterStore.count }}</h1>
    <button @click="counterStore.increment">Add B</button>
  </div>
</template>
