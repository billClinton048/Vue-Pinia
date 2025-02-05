
<template>
  <div class="flex flex-col justify-center items-center">
    <h1 class="text-8xl text-center p-10">
      {{ storeCounter.count }}
    </h1>
    <div>
      <button @click = "storeCounter.decreaseCount" class="text-8xl"> - </button>
      <button @click = "storeCounter.increaseCount" class="text-8xl m-5"> + </button>

    </div>
    </div>
      <hr>
      <div class="py-5">
        This is : {{ storeCounter.oddOrEven }}
      </div>
      <hr>
      <div>
        <h3>Edit Counter: </h3>
        <input class="border-black border" v-model="storeCounter.count" type="number">
      </div>

</template>

<script setup>
// import store
import { useCounterStore } from '@/stores/counter'

// Assigning store to Variable
const storeCounter = useCounterStore()

</script>
