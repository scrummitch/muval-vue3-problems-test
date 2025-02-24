<script setup lang="ts">
import { useCounterStore } from '@/stores/counter'

const counterStore = useCounterStore()
</script>

<template>
  <div class="grid">
    <code>PiniaCompA.vue</code>
    <pre>{{ counterStore }}</pre>
    <h1 class="text-4xl">{{ counterStore.count }}</h1>
    <button @click="counterStore.increment">Add A</button>
  </div>
</template>
