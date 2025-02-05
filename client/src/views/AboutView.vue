<template>
  <div class="m-10 text-center text-6xl">
    <h1>
      About
    </h1>
    <h2>
      {{ storeCounter.count}}
    </h2>
  </div>
</template>

<script setup>
// import store
import { useCounterStore } from '@/stores/counter'

// Assigning store to Variable
const storeCounter = useCounterStore()
</script>