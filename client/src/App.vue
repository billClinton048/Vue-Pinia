<template>
  <div class="text-center text-2xl">
  <nav>
    <RouterLink to="/">HOME</RouterLink> |
    <RouterLink to="/about">ABOUT</RouterLink>
  </nav>

   <RouterView />
    </div>
</template>

<script setup>
import { RouterView } from 'vue-router';


</script>

<style scoped>

</style>